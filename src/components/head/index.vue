<template>
	<div class="c-header">
		<ul class="header-ul"><li>推荐</li><li>课程</li><li>实战</li><li>职业路线</li><li class="header-search"><img src="../../assets/search.png"></li><li class="header-history"><img src="../../assets/history.png"></li>
		</ul>
	</div>
</template>

<style scoped>  
/*scoped的意思是写的样式仅在组件内有效，在这个组件外面就无效了*/
	.c-header{
		position:fixed;           /*固定位置*/
		top:0;				/*使div始终在顶部*/
		z-index: 3;			/*使页面始终在最上面*/
		width: 375px;		
		font-size:0;
		box-shadow: 0px 2px 5px #000;
		background: white;
	}
	.header-ul li{
		display:inline-block;   /*使li有行内元素的属性*/
		padding-left: 20px;
		font-size: 20px;
		line-height: 78px;

	}
	img{
		width:18px;
	}
</style>

