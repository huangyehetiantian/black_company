<template>
	<view >
		<div  v-for='item in lists' class="list ">
					
						
						 <div class ="flexbetween">
						 	<span >{{item.title}} </span>
						 	<span ><span  class="mr10">{{item.name}} </span>{{item.time}} </span>
						 </div>   
						 <div class="article flexbetween">
						 	<div>{{item.article}}</div>
							
						 </div>
						
					 </div>
		      
						 
		</div>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello',
				lists: [
					{
					title: "前端必备技能",
					article: "硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师....",
				    time:"2021/4/1",
					name: "佚名"
				    },
					{
					title: "前端必备技能",
					article: "硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师....",
					time:"2021/4/1",
					name: "佚名"
					},
					{
					title: "前端必备技能",
					article: "硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师硬件技能+软件技能是所有开发工程师....",
					time:"2021/4/1",
					name: "佚名"
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

	.article{
		font-size:12px;
		margin-top:10px;
		justify-content: flex-start;
		color:#333
	}
     .mr10{
		 margin-right:10px;
	 }
</style>
