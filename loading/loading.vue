<template>
	<section v-show="zg">
		<div class="mock" v-show="loading">
			<div class="lds-css ng-scope">
				<div class="lds-spinner" style="width:100%;height:100%">
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
					<div></div>
				</div>
			</div>
		</div>
		<div class="mockb" v-show="loadingb">
			<div class="loader font1">
				<span>情</span>
				<span class="span2">话</span>
				<span class="span3">搜</span>
				<span class="span4">素</span>
				<span class="span5">中</span>
				<span class="span6">.</span>
				<span class="span7">.</span>
				<span class="span8">.</span>
			</div>
		</div>
		<div class="mockb" v-show="loadingc">
			<div class="loader font1">
				<span>请</span>
				<span class="span2">稍</span>
				<span class="span3">等</span>
				<span class="span4">一</span>
				<span class="span5">会</span>
				<span class="span6">.</span>
				<span class="span7">.</span>
				<span class="span8">.</span>
			</div>
		</div>
		<div class="mockc" v-show="loadingd">
			<div class="loaderb loader-13">
				<div class="css-heart heart1"></div>
				<div class="css-heart heart2"></div>
				<div class="css-heart heart3"></div>
				<div class="css-heart heart4"></div>
			</div>
		</div>
	</section>
</template>
<style>
section {
	/*    width:100vh;
        height:100vh;*/
    background: #c3c1f6;
    width: 100%;
    height: 100%;
    position: relative;
}
.lds-css {
	display: flex;
	margin: auto;
	height: 100%;
}

.lds-spinner {
	margin: auto;
}
.mock {
	position: fixed;
	z-index: 100;
	background-color: #abb2bf;
	top: 0;
	left: 0;
	width: 100%;
	z-index: 132132;
	height: 100%;
}
.mockb {
	position: fixed;
	z-index: 100;
	background: url(../assets/img/loading.png) no-repeat;
	background-size: 100% 100%;
	width: 10rem;
	height: 15.14rem;
	top: 0;
	left: 0;
	z-index: 132132;
	font-family: 'fzxj';
	font-size: 48px;
	color: #ffffff;
	line-height: 15.14rem;
}
.mockc {
	position: fixed;
	z-index: 100;
	background: #c3c1f6;
	background-size: 100% 100%;
	width: 10rem;
	height: 15.14rem;
	top: 0;
	left: 0;
	z-index: 132132;
	font-family: 'fzxj';
	font-size: 48px;
	color: #ffffff;
	line-height: 15.14rem;
}
.loader {
	overflow: hidden;
	position: absolute;
	left: 50%;
	width: 4rem;
	margin-left: -2rem;
}
.loader span {
	-moz-animation: loading 1s linear infinite -0.8s;
	-webkit-animation: loading 1s linear infinite -0.8s;
	animation: loading 1s linear infinite -0.8s;
	float: left;
}
.loader .span2 {
	-moz-animation: loading 1s linear infinite -0.2s;
	-webkit-animation: loading 1s linear infinite -0.2s;
	animation: loading 1s linear infinite -0.2s;
}
.loader .span3 {
	-moz-animation: loading 1s linear infinite -0.5s;
	-webkit-animation: loading 1s linear infinite -0.5s;
	animation: loading 1s linear infinite -0.5s;
}
.loader .span4 {
	-moz-animation: loading 1s linear infinite -1.1s;
	-webkit-animation: loading 1s linear infinite -1.1s;
	animation: loading 1s linear infinite -1.1s;
}
.loader .span5 {
	-moz-animation: loading 1s linear infinite -0.36s;
	-webkit-animation: loading 1s linear infinite -0.36s;
	animation: loading 1s linear infinite -0.36s;
}
.loader .span6 {
	-moz-animation: loading 1s linear infinite -0.65s;
	-webkit-animation: loading 1s linear infinite -0.65s;
	animation: loading 1s linear infinite -0.65s;
}
.loader .span7 {
	-moz-animation: loading 1s linear infinite -0.93s;
	-webkit-animation: loading 1s linear infinite -0.93s;
	animation: loading 1s linear infinite -0.93s;
}
.loader .span7 {
	-moz-animation: loading 1s linear infinite -1.3s;
	-webkit-animation: loading 1s linear infinite -1.3s;
	animation: loading 1s linear infinite -1.3s;
}
@-moz-keyframes loading {
	0%,
	100% {
		-moz-transform: scale(1) rotateZ(0deg);
		transform: scale(1) rotateZ(0deg);
		opacity: 1;
	}

	26% {
		-moz-transform: scale(1.1) rotateZ(12deg);
		transform: scale(1.1) rotateZ(12deg);
		opacity: 0.2;
	}

	76% {
		-moz-transform: scale(0.8) rotateZ(-8deg);
		transform: scale(0.8) rotateZ(-8deg);
		opacity: 0.6;
	}
}
@-webkit-keyframes loading {
	0%,
	100% {
		-webkit-transform: scale(1) rotateZ(0deg);
		transform: scale(1) rotateZ(0deg);
		opacity: 1;
	}

	26% {
		-webkit-transform: scale(1.1) rotateZ(12deg);
		transform: scale(1.1) rotateZ(12deg);
		opacity: 0.2;
	}

	76% {
		-webkit-transform: scale(0.8) rotateZ(-8deg);
		transform: scale(0.8) rotateZ(-8deg);
		opacity: 0.6;
	}
}
@keyframes loading {
	0%,
	100% {
		-moz-transform: scale(1) rotateZ(0deg);
		-ms-transform: scale(1) rotateZ(0deg);
		-webkit-transform: scale(1) rotateZ(0deg);
		transform: scale(1) rotateZ(0deg);
		opacity: 1;
	}

	26% {
		-moz-transform: scale(1.1) rotateZ(12deg);
		-ms-transform: scale(1.1) rotateZ(12deg);
		-webkit-transform: scale(1.1) rotateZ(12deg);
		transform: scale(1.1) rotateZ(12deg);
		opacity: 0.2;
	}

	76% {
		-moz-transform: scale(0.8) rotateZ(-8deg);
		-ms-transform: scale(0.8) rotateZ(-8deg);
		-webkit-transform: scale(0.8) rotateZ(-8deg);
		transform: scale(0.8) rotateZ(-8deg);
		opacity: 0.6;
	}
}

.lds-spinner {
	position: relative;
}

.lds-spinner div {
	left: 94px;
	top: 49px;
	position: absolute;
	-webkit-animation: lds-spinner linear 1s infinite;
	animation: lds-spinner linear 1s infinite;
	background: #0099e5;
	width: 12px;
	height: 22px;
	border-radius: 40%;
	-webkit-transform-origin: 6px 51px;
	transform-origin: 6px 51px;
}

.lds-spinner div:nth-child(1) {
	-webkit-transform: rotate(0deg);
	transform: rotate(0deg);
	-webkit-animation-delay: -0.916666666666667s;
	animation-delay: -0.916666666666667s;
}

.lds-spinner div:nth-child(2) {
	-webkit-transform: rotate(30deg);
	transform: rotate(30deg);
	-webkit-animation-delay: -0.833333333333333s;
	animation-delay: -0.833333333333333s;
}

.lds-spinner div:nth-child(3) {
	-webkit-transform: rotate(60deg);
	transform: rotate(60deg);
	-webkit-animation-delay: -0.75s;
	animation-delay: -0.75s;
}

.lds-spinner div:nth-child(4) {
	-webkit-transform: rotate(90deg);
	transform: rotate(90deg);
	-webkit-animation-delay: -0.666666666666667s;
	animation-delay: -0.666666666666667s;
}

.lds-spinner div:nth-child(5) {
	-webkit-transform: rotate(120deg);
	transform: rotate(120deg);
	-webkit-animation-delay: -0.583333333333333s;
	animation-delay: -0.583333333333333s;
}

.lds-spinner div:nth-child(6) {
	-webkit-transform: rotate(150deg);
	transform: rotate(150deg);
	-webkit-animation-delay: -0.5s;
	animation-delay: -0.5s;
}

.lds-spinner div:nth-child(7) {
	-webkit-transform: rotate(180deg);
	transform: rotate(180deg);
	-webkit-animation-delay: -0.416666666666667s;
	animation-delay: -0.416666666666667s;
}

.lds-spinner div:nth-child(8) {
	-webkit-transform: rotate(210deg);
	transform: rotate(210deg);
	-webkit-animation-delay: -0.333333333333333s;
	animation-delay: -0.333333333333333s;
}

.lds-spinner div:nth-child(9) {
	-webkit-transform: rotate(240deg);
	transform: rotate(240deg);
	-webkit-animation-delay: -0.25s;
	animation-delay: -0.25s;
}

.lds-spinner div:nth-child(10) {
	-webkit-transform: rotate(270deg);
	transform: rotate(270deg);
	-webkit-animation-delay: -0.166666666666667s;
	animation-delay: -0.166666666666667s;
}

.lds-spinner div:nth-child(11) {
	-webkit-transform: rotate(300deg);
	transform: rotate(300deg);
	-webkit-animation-delay: -0.083333333333333s;
	animation-delay: -0.083333333333333s;
}

.lds-spinner div:nth-child(12) {
	-webkit-transform: rotate(330deg);
	transform: rotate(330deg);
	-webkit-animation-delay: 0s;
	animation-delay: 0s;
}

.lds-spinner {
	width: 200px !important;
	height: 200px !important;
	-webkit-transform: translate(-100px, -100px) scale(1) translate(100px, 100px);
	transform: translate(-100px, -100px) scale(1) translate(100px, 100px);
}
.loaderb {
	position: relative;
	width: 60px;/*no*/
	height: 60px;/*no*/
	border-radius: 50%;
	margin: 75px;
	display: inline-block;
	vertical-align: middle;
}

.loader-13 .css-heart {
	position: absolute;
	-webkit-animation: star-fly-out 1s ease alternate infinite;
	animation: star-fly-out 1s ease alternate infinite;
	-webkit-transform: scale(0.2);
	transform: scale(0.2);
}
.loader-13 .heart1 {
	top: 0;
	left: 30px;
}
.loader-13 .heart2 {
	left: 60px;
	top: 30px;
}
.loader-13 .heart3 {
	top: 60px;
	left: 30px;
}
.loader-13 .heart4 {
	left: 0;
	top: 30px;
}
.css-heart:before,
.css-heart:after {
	position: absolute;
	content: '';
	left: 50px;/*no*/
	top: 0;
	width: 50px;/*no*/
	height: 80px;/*no*/
	background: #323080;
	border-radius: 50px 50px 0 0;/*no*/
	-webkit-transform: rotate(-45deg);
	transform: rotate(-45deg);
	-webkit-transform-origin: 0 100%;
	transform-origin: 0 100%;
}
.css-heart:after {
	left: 0;
	-webkit-transform: rotate(45deg);
	transform: rotate(45deg);
	-webkit-transform-origin: 100% 100%;
	transform-origin: 100% 100%;
}
@keyframes star-fly-out {
	0% {
		top: 19px; /*no*/
		left: 19px; /*no*/
	}
	100% {
	}
}
</style>
<script>
export default {
	name: 'loading',
	data() {
		return {
			zg:false,
			loading: false,
			loadingb: false,
			loadingc: false,
			loadingd: false
		};
	},
	created() {
		var that = this;
		this.bus.$on('loading', function(data,datab) {
			// console.log(data);
			that.loading = !!data;
			that.zg=!!datab;
		});
		this.bus.$on('loadingb', function(data,datab) {
			// console.log(data);
			that.loadingb = !!data;
			that.zg=!!datab;
		});
		this.bus.$on('loadingc', function(data,datab) {
			// console.log(data);
			that.loadingc = !!data;
			that.zg=!!datab;
		});
		this.bus.$on('loadingd', function(data,datab) {
			// console.log(data);
			that.loadingd = !!data;
			that.zg=!!datab;
		});
	}
};
</script>
