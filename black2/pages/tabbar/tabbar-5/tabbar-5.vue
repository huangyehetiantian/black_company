<template>
	<view >
		<div class="bgimg">
			<div class="myimg"></div>
			<div class="name">Only</div>
			<div class="edit"><image src="../../../static/img/release.png"></image></div>
		</div>
		<div class="header">
			关注机构
		</div>
		<div class="header">
			我的评论
		</div>
		<div class="header">
			我的文章
		</div>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.bgimg {
		width:100%;
		height:300px;
		background: url(../../../static/bg.jpeg) center center ;
		position:relative;
	}
	.myimg{
		width:80px;
		height:80px;
		border-radius: 100%;
		background:#007AFF;
        position:absolute;
		bottom:50px;
		left:10px;
	}
	.name{
		position:absolute;
		bottom:80px;
		left:100px;
		font-size:24px;
		color:white;
	}
	.edit{
		position:absolute;
		bottom:60px;
		right:10px;
		font-size:18px;
		color:#007AFF;
	}
	.edit image{
		width:40px;
		height:40px;
	}
	.header{
		height:60px;
		line-height:60px;
		text-align:left;
		padding-left:20px;
	}
</style>
