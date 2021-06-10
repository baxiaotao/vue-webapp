<template>
	<div class="c-container">
		<ul class="c-footer">
			<li>
				<img src="@/assets/home.png">
				<p>首页</p>
			</li>
			<li>
				<img src="@/assets/sea.png">
				<p>发现</p>
			</li>
			<li>
				<img src="@/assets/download.png">
				<p>下载</p>
			</li>
			<li>
				<img src="@/assets/me.png">
				<p>我的</p>
			</li>
		</ul>
	</div>
</template>
<script type="text/javascript">
	export default{
		data(){
			return{

			}
		}
	}
</script>
<style scoped>
*{
	margin: 0;
	padding:0;
}
	.c-container{
		position: fixed;
		bottom:0;
		background-color:white;
		border: 1px gray solid;
		box-shadow: 0px 2px 5px #000;
	}

	.c-footer{
		width:375px;
		display: flex;
		justify-content: space-between;	}
	.c-footer li{
		direction:row;
		align-items: center;

	}
	.c-footer li p{
		font-size: 10px;

	}
	.c-footer li img{
		width:24px;

	}
</style>
