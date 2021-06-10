<template>
	<div class="home-page">
		
		<v-head></v-head>
		<ul class="nav">
			<li v-for="item in ArrayList">
				<img :src="item.imgUrl">
				<span>{{item.name}}</span>
			</li>
		</ul>
		<v-course :arrList="array"></v-course>
		<v-footer></v-footer>
	</div>

</template>

<script>
	import Head from '@/components/head'; //使用组件的两部曲：
	import imgUrl1 from '@/assets/web.png';
	import imgUrl2 from '@/assets/webservice.png';
	import imgUrl3 from '@/assets/move.png';
	import imgUrl4 from '@/assets/data.png';
	import imgUrl5 from '@/assets/bigdata.png';
	import Course from '@/components/course';
	import course1 from '@/assets/course1.jpg';
	import course2 from '@/assets/course2.jpg';
	import course3 from '@/assets/course3.jpg';
	import course4 from '@/assets/course4.jpg';
	import course5 from '@/assets/course5.jpg';
	import footer from '@/components/footer';
	 export default{
	 	data(){
	 		return{
	 			ArrayList:[],
	 			arrList:[]
	 			
	 		}
	 	},
	 	mounted(){
	 		this.ArrayList = [
	 		{
	 			imgUrl:imgUrl1,
	 			name:"前端开发"
	 		}
	 		,
	 		{
	 			imgUrl:imgUrl2,
	 			name:"后端开发"
	 		}
	 		,
	 		{
	 			imgUrl:imgUrl3,
	 			name:"移动开发"
	 		},
	 		{
	 			imgUrl:imgUrl3,
	 			name:"数据库"
	 		},
	 		{
	 			imgUrl:imgUrl4,
	 			name:"云计算"
	 		}];

	 		this.array=[
	 		{
	 			imgUrl:course1,
	 			title:"c语言",
	 			msg:"100人在学"
	 		},
	 		{
	 			imgUrl:course2,
	 			title:"Java",
	 			msg:"100人在学"
	 		},
	 			 		
	 		{
	 			imgUrl:course3,
	 			title:"c#",
	 			msg:"1000人在学"
	 		},
	 		{
	 			imgUrl:course4,
	 			title:"python",
	 			msg:"100人在学"
	 		},	 		
	 		{
	 			imgUrl:course5,
	 			title:"vue.js",
	 			msg:"1000人在学"
	 		},
	 		]

	 	
	 	},
	 	components:{
	 		'v-head':Head,
	 		'v-course':Course,
	 		'v-footer':footer
	 	}
	 }  
											// 1：导入组件
											//2：注册组件


</script>
<style scoped>
	.nav{
		height: 100px;
		padding-top:77px;
		overflow-x: scroll;
		white-space: nowrap;
		font-size: 0;
		background-color: #F3F5F7;
	}
	.nav li{
		width: 88px;
		display: inline-block;
		text-align: center;
		font-size:14px;
	}
	img{
		display: block;
		width: 32px;
		margin:20px auto 12px;
	}
</style>