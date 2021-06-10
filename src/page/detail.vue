<template>
	<div class="detail-page">
		<video controls="controls"></video>
		<div class="return1"><</div>
		<div>
			<ul class="nav">
				<li v-for="item in arr">{{item}}</li>
			</ul>
		</div>
		<div class="title">
			<h1>{{title}}</h1>
			<p>{{des}}</p>
		</div>
	</div>
</template>
 <script type="text/javascript">
 	export default{
 		data(){
 			return{
 				arr:[],
 				title:"",
 				des:""
 			}
 		},
 		mounted(){
 			this.arr = ["详情","更多","评论","lala"];
 			this.title = "这里是标题，这里的内容是从服务器中获取的；";
 			this.des = "这里是描述，这里的内容是从服务器中获取的";

 		}
 	}
 </script>
<style scoped>
	.detail-page{
		width:20px;
	}

	video{
		width:375px;
		z-index: 1;
		position: relative;
	}
	.return1{
		width:20px;
		height: 20px;
		color:white;
		z-index: 3;
		
	}
	.nav{
		width:375px;
		height:80px;
		border:1px gray solid;
		display: flex;
		justify-content: space-between; /*将容器内部的元素程两端分布*/
		align-items: center;
		position: absolute;
		top:179px;


	}
	.nav li{
		display: inline-block;
		font-size: 25px;
		color:gray;
	}
	.title{
		width:375px;
		height:200px;
		position:absolute;
		top:260px;
		border: 2px gray solid;

	}
	.title h1{
		font-size: 30px;

	}
	.title p{
		font-size:25px;
	}
</style>