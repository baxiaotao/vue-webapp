<template>
	<div> 
		<ul class="c-course">
		<router-link to="/detail">
			<li v-for="item in arrList">
			<img :src="item.imgUrl">
			<h1>{{item.title}}</h1>
			<p>{{item.msg}}</p>
			</li>
		</router-link>
		</ul>
	</div>
</template>

<script>
	export default{
		props:{
			arrList:Array
		}
	}
</script>

<style scoped>
	.c-course{
		padding:24px 0;
		background:#fff;
		position:absolute;
		left: 10px;

	}
	.c-course li{
		width: 335px;
		height: 72px;
		position: relative;
		margin :0 auto 24px;
		border: 2px gray solid;
	}
	.c-course li img{
		position: absolute;
		width: 108px;
		border-radius: 5px;
		top:5px;
	}
	.c-course h1{
		font-size: 15px;
		padding-left: 124px;
	}
	.c-course li p{
		font-size: 10px;
		padding-left: 128px;
		color:gray;
	}
</style>