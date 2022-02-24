<template>
	<div class="Home">
		<button @click="counter.increment">You have clicked me {{ counter.count }} times</button>
	</div>
</template>

<script lang="ts" setup>
import { useCounterStore } from '@/stores/counter'
const counter = useCounterStore()
/* JS / TS */
</script>

<style lang="scss" scoped>
/* CSS / SCSS */
.Home {
	height: 100vh;
	width: 100vw;
	display: flex;
	align-items: center;
	justify-content: center;
	background: rgb(229, 232, 238);

	button {
		border: none;
		padding: 15px 20px;
		background: #41B883;
		color: #FFFFFF;
		cursor: pointer;
		border-radius: 5px;
	}
}

</style>
