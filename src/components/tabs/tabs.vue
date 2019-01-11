<template>
	<div id="tabsContainer">
		<ul class="tabsList">
			<li class="tabsItem tabsActive">首页</li>
			<li class="tabLine">|</li>
			<li class="tabsItem">酒店<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">旅游<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">跟团游</li>
			<li class="tabLine">|</li>
			<li class="tabsItem">自由行</li>
			<li class="tabLine">|</li>
			<li class="tabsItem">机票<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">火车<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">汽车票<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">用车<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">门票<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">攻略</li>
			<li class="tabLine">|</li>
			<li class="tabsItem">全球购<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">礼品卡<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">商旅</li>
			<li class="tabLine">|</li>
			<li class="tabsItem">游轮<span class="downArrow"></span></li>
			<li class="tabLine">|</li>
			<li class="tabsItem">目的地</li>
			<li class="tabLine">|</li>
			<li class="tabsItem">更多<span class="downArrow"></span></li>
			<li class="lastItem tabsDiv">
				<div class="top">
					<span class="login">登录</span>
					<span class="districtLine">|</span>
					<span class="register">注册</span>
				</div>
				<div class="bottom">
					<span class="myctrip">我的携程</span>
					<span class="downArrow"></span>
				</div>
			</li>
		</ul>
	</div>
</template>

<script>
	export default {
		data() {
			let msg = "tabs";
			return {
				msg: msg
			};
		}
	}
</script>

<style scoped>
	#tabsContainer {
		width: 100%;
		height: 40px;
		background-color: #2577e3;
		margin: 0 auto 15px;
	}
	@media screen and (max-width: 1200px) {
		.tabsList{
			min-width: 980px;
		}
	}
	.tabsList{
		margin: 0px;
		padding: 0px;
		list-style: none;
		/* width: 100%; */
		height: 40px;
		min-width: 980px !important;
		max-width: 1180px;
		margin: 0 auto;
	}
	.tabsList li{
		display: inline-block;
		float: left;
	}
	.tabsList .tabsItem{
		line-height: 40px;
		height: 40px;
		color: #fff;
		padding: 0px 8px;
		cursor: pointer;
		font-size: 15px;
	}
	.tabsList .tabsItem:hover{
		background-color: #0a56bb;
	}
	.tabsList .tabsItem:hover .downArrow{
		transform: rotate(180deg);
	}
	.tabsList .tabsActive{
		background-color: #0a56bb;
	}
	.tabsList .tabsDiv{
		width: 128px;
	}
	.tabLine{
		width: 1px;
		height: 20px;
		line-height: 40px;
		color: #1d67dd;
		clear: none;
		border: none;
	}
	.downArrow{
		display: inline-block;
		width: 0;
		height: 0;
		overflow: hidden;
		line-height: 0;
		font-size: 0;
		margin-left: 5px;
		vertical-align: middle;
		border-top: 3px solid #fff;
		border-bottom: 0 none;
		border-left: 3px solid transparent;
		border-right: 3px solid transparent;
	}
	.lastItem{
		width: 126px;
		height: 40px;
		/* background-color: #ff9913; */
		background: #ff9913 url(../../assets/un_header_footer20160610.png) no-repeat -59px -179px;
		margin-left: 7px;
		color: #fff;
		font-size: 15px;
	}
	.top, .down{
		padding-left: 27px;
		height: 20px;
		line-height: 20px;
		font-size: 12px;
	}
	.login, .register, .myctrip{
		cursor: pointer;
	}
	.bottom:hover .downArrow{
		transform: rotate(180deg);
	}
	.myctrip{
		margin-left: 7px;
		font-size: 13px;
	}
</style>
