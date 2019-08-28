<!-- 首页 三图广告 -->
<template>
	<!-- 左边：w373 h530 -->
	<!-- 右边：w375 h263 边h2 -->
	<view class="d-flex">
		<image :src="resdata.big.src" 
		lazy-load
		style="width: 373upx;height: 530upx;border-right: 2upx solid #F5F5F5;" @tap="event(resdata.bg)"></image>
		<view class="d-flex flex-column">
			<image :src="resdata.smalltop.src" 
			style="width: 375upx;height: 264upx;border-bottom: 2upx solid #F5F5F5;"
			@tap="event(resdata.smalltop)"></image>
		<image :src="resdata.smallbottom.src"
		style="width: 375upx;height: 264upx;" @tap="event(resdata.smallbottom)"></image>
		</view>
	</view>
</template>

<script>
	export default{
		props:{
			resdata:Object
		},
		methods:{
			event(obj){
				console.log("点击了"+ obj)
			}
		}
	}
</script>

<style>
</style>
