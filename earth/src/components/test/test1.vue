<template>
	<div>
		<div>{{total_price}}</div>
		<input type="text" v-model="commodity.num">
	</div>
</template>

<script>
export default {
	name: "Test1",
	data() {
		return{
			commodity: {
				price: Number= 12,
				num: Number= 0
			}
		}
	},
	computed: {
		'total_price': function(){
			return this.commodity.num * this.commodity.price;
		}
	}
}
</script>

<style lang="less">
	
</style>