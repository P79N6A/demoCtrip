<template>
	<div class="searchContainer">
		<div class="searchLeft">
			<img src="../../assets/c_logo2013.png">
			<div class="cui_search">
				<input type="text" value="" class="leftInput" placeholder="搜索旅行地/酒店/旅游/景点门票/交通"/>
				<button class="searchBtn"></button>
			</div>
		</div>
		<div class="searchRight">
			<ul class="rightList">
				<li class="rightItem">
					<span class="globalImg"></span>
					<span class="itemText">Language</span>
					<span class="downArraw"></span>
				</li>
				<li class="rightItem rightLine">|</li>
				<li class="rightItem">
					<span class="itemText">客服中心</span>
				</li>
				<li class="rightItem rightLine">|</li>
				<li class="rightItem">
					<span class="itemText">境内&nbsp;:&nbsp;</span>
					<span class="phoneNum">95010</span>
					<span class="downBlueArraw"></span>
				</li>
				<li class="rightItem">
					<span class="iphone"></span>
				</li>
				<li class="rightItem">
					<span class="wechat"></span>
				</li>
			</ul>
		</div>
	</div>


</template>

<script>
	export default {
		// name: "headerContainer",
		data() {
			const item = {
				date: '2019-01-10',
				name: 'Tom',
				address: '中大银座'
			}
			return {
				tableData: Array(20).fill(item)
			};
		}
	}
</script>

<style scoped>
	.searchContainer{
		width: 61%;
		margin-left: auto;
		margin-right: auto;
		margin-top: 5px;
		margin-bottom: 5px;
		height: 53px;
		display: -webkit-box;
		display: -webkit-flex;
		display: -moz-box;
		display: -ms-flexbox;
		display: flex;
		justify-content: space-between;
	}
	.searchLeft{
		
	}
	.searchLeft img{
		width: 126px;
		height: 43px;
		margin-top: 5px;
		float: left;
	}
	.searchLeft .cui_search{
		margin: 11px 0;
		margin-left: 50px;
		float: left;
		height: 28px;
		line-height: 28px;
		position: relative;
	}
	.leftInput{
		border: 1px solid #a4cbff;
		border-radius: 5px;
		width: 325px;
		height: 28px;
		box-sizing: border-box;
		padding-right: 45px;
		box-shadow: 2px 2px 1px 0 rgba(164, 203, 255, 0.25) inset;
    outline: 0 none;
	}
	.searchBtn{
		position: absolute;
		top: 3px;
		right: 1px;
		width: 42px;
		height: 26px;
		border: 0 none;
		cursor: pointer;
		background-image: url(../../assets/un_header_footer20160610.png);
		background-repeat: no-repeat;
		background-position: -52px -603px;
		background-color: #a4cbff;
	}
	.searchRight{
		
	}
	.rightList{
		margin: 0px;
		padding: 0px;
		list-style: none;
		height: 53px;
		line-height: 53px;
	}
	.rightItem{
		display: inline-block;
		cursor: pointer;
	}
	.rightItem .globalImg{
		display: inline-block;
		width: 20px;
		height: 20px;
		background-image: url(../../assets/un_header_footer20160610.png);
		background-repeat: no-repeat;
		background-position: -64px 0;
		position: relative;
		top: 7px;
	}
	.rightItem .downArraw{
		display: inline-block;
		width: 13px;
		height: 13px;
		background-image: url(../../assets/un_header_footer20160610.png);
		background-repeat: no-repeat;
		background-position: -63px -260px;
		position: relative;
		top: 7px;
	}
	.rightItem .downBlueArraw{
		display: inline-block;
		width: 13px;
		height: 13px;
		background-image: url(../../assets/un_header_footer20160610.png);
		background-repeat: no-repeat;
		background-position: -22px -264px;
		position: relative;
		top: 7px;
	}
	.rightItem .iphone{
		display: inline-block;
		width: 20px;
		height: 20px;
		background-image: url(../../assets/un_header_footer20160610.png);
		background-repeat: no-repeat;
		background-position: 0 -56px;
		position: relative;
		top: 7px;
	}
	.rightItem .wechat{
		display: inline-block;
		width: 20px;
		height: 20px;
		background-image: url(../../assets/un_header_footer20160610.png);
		background-repeat: no-repeat;
		background-position: -20px -55px;;
		position: relative;
		top: 7px;
	}
	.rightItem .itemText{
		display: inline-block;
		color: #4c4c4c;
		font-size: 12px;
	}
	.rightLine{
		color: #b2b2b2;
		cursor: default;
	}
	.rightItem .phoneNum{
		color: #06c;
		font-style: normal;
		font-size: 12px;
	}
	
</style>
