<template>
	 
	<!-- 輪	播图 -->
	<!--<view><swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000" :circular="true">
		<swiper-item v-for="() in">
			<image src="" mode=""></image>
		</swiper-item>
	</swiper>
	</view> -->
	<!-- 導航区 -->
	<view class="scroll">
		<!-- 左   每一項為一個view-->
		<scroll-view class="left"cscroll-y>
          <view class="active">熱銷</view>
		  <view>折扣</view>
		  <view>廚師推介</view>
		  <view>超值套歺</view>
		  <view>湯麵</view>
		  <view>小炒</view>
		  <view>白飯</view>
		  
		</scroll-view>
		<!-- 右 -->
		<view></view>
	</view>
</template>

<script>
	
	components:{
	   
	};
	export default {
		data() {
			return {
				goods_info:{}
			}
		},
		onLoad() {
		},
		methods: {
			
			// async getScrollCate(){
			// 	const res = avait this.$myRuquest({url:'/api/getimegcategory'})}
			
		}
	}
	   </script>

<style lang="scss">
	// page{
	// 	height: 100%;}
	.scroll{
		height: 100%;
	}
	.left{
		height: 100%;
		width: 200rpx;
		border-right:1px solid #ddd ;
		.active{
			background:#FFEB3B;
			color: #fff;
		}
		view{
			height: 60px;
			line-height: 60px;
			color:#333;
			text-align: center;
			font-size: 40rpx;
			border-top:1px solid #ddd ;
			
		}
		
	}
</style>
