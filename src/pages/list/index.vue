<template>
	<view class="listWrap">
		<view class="list" v-for="(item, index) in listData" @click="listHandle(item.id)" :key="index">
			<view>
			<image mode="widthFix" :src="item.imgSrc"></image>
			</view>
			<text>{{item.text}}</text>
		</view>
	</view>
</template>

<script lang="ts">
	export default {
		data() {
			return {
				listData: [
					{
						id: 1,
						imgSrc: '/static/pic1.jpeg',
						text: '西柏坡红色旅游区'
					},
					{
						id: 2,
						imgSrc: '/static/pic2.gif',
						text: '井陉万人坑纪念馆'
					},
					{
						id: 3,
						imgSrc: '/static/pic3.gif',
						text: '梅花惨案纪念馆'
					}
				]
			}
		},
		onLoad() {

		},
		methods: {
			listHandle(id) {
				uni.navigateTo({
					url: '/pages/detail/index?id=' + id
				})
				console.log();
				
			},
		}
	}
</script>

<style>
.list {
  margin: 15px;
  background: #fff;
  padding-bottom: 15px;
  border: 1px solid #ddd;
  box-shadow: 0 0 5px #ddd;
}

.list image {
  width: 100%;
  display: block;
  margin-bottom: 15px;
}

.list text {
  padding: 15px;
}
</style>
