<template>
  <transition name="fade">
    <div class="r-tip" v-if="visible">
      <span class="r-tip-text" v-html="message"></span>
    </div>
  </transition>
</template>

<script>
	export default {
    props: {
      message: String
    },
    data () {
      return {
        visible: false
      }
    }
  }
</script>

<style>
	.r-tip {
	  position: fixed;
	  max-width: 80%;
	  padding: 20PX;
	  border-radius: 5PX;
	  background: rgba(0, 0, 0, 0.7);
	  color: #fff;
	  box-sizing: border-box;
	  text-align: center;
	  z-index: 9999;
	  left: 50%;
	  top: 50%;
	  transform: translate(-50%, -50%);
	}
	.r-tip-text{
	  font-size: 16PX;
	  display: block;
	  text-align: center;
	}
	.fade-enter-active, .fade-leave-active {
	  transition: opacity .3s;
	}
	.fade-enter, .fade-leave-to {
	  opacity: 0;
	}
</style>
