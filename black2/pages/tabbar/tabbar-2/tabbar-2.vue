<template>
	<view >
		<div  v-for='item in whitelists' class="list flexStart">
					  <image src="../../../static/img/123.png" class="image"></image>
					 <div >
						
						 <div class ="flexbetween">
						 	<span >{{item.name}} </span>
						 	<image src="../../../static/img/tabbar/guanzhuactive.png" class="loveimg"></image>
						 </div>   
						 <div class="address flexbetween">
						 	<div>地址：{{item.address}}</div>
							<div  class="start ml5">
								<span v-for="item in item.start">🌟</span> 
							</div>
						 </div>
						 <div class="assess">评价：{{item.assess}}</div>
					 </div>
		      
						 
		</div>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello',
				whitelists: [
					{
					name: "青岛XXX公司",
					address: "市北凯德mall",
					start:5,
					assess:"凑合吧"
				    }
				]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.address_header{
		height:40px;
		text-align:left;
		line-height:40px;
		padding-left:2%
	}
	.flexStart{
		display:flex;
		justify-content: flex-start;
	}
	.image{
		width:100px;
		height:100px;
	}
	.ml5{
		margin-left:5px;
	}
	.list{
		text-align: left;
		width:98%;
		margin:6px auto;
		font-size:12px;
		padding:1% 2%;
		background:white;
		border:1px solid #eee;
		box-sizing: border-box;
	}
	.flexbetween{
		display: flex;
		justify-content: space-between;
		font-size:14px;
		margin-bottom:10px;
	}
	.start{
		display:inline-block;
		width:100px;
		color:#e6e6e6
	}
	.title{
		height:40px;
		line-height: 40px;
		text-align: left;
		color:#2c3e50;
		padding-left:2%;
		display:flex;
		justify-content: space-between;
		padding-right:2%;
	}
	.more{
		color:#007AFF;
		font-size:12px;
	}
	.more:hover{
		color: red;
		cursor:pointer;
		
	}
	.assess{
		font-size:12px;
		margin-top:10px;
		justify-content: flex-start;
	}
	.mt20{
		margin-top:20px;
	}
	.love{
		color:red;
		font-size:12px;
		cursor:pointer
	}
	.love:hover{
		font-size:14px;
	}
	.loveimg{
		width:30px;
		height:30px;
	}
</style>
