<style lang="stylus">
	*
		margin 0
		padding 0
		line-height 1
		font-family Microsoft Yahei, sans-serif, Arial
		box-sizing border-box
	ul
	ol
		list-style none
	a
		text-decoration none
		color inherit
	b
		font-weight normal
	em
	i
		font-style normal
	input
		outline none
	textarea
		resize none
	body
		background-color #efeff4
	.icon
		width 1.2rem
		height 1.2rem
		fill currentColor
		overflow hidden
</style>
<template>
	<div>
		<router-view />
		<my-footer />
	</div>
</template>
<script>
	import MyFooter from "./components/Footer";
	export default {
		components: {
			MyFooter
		},
		beforeCreate(){
			document.documentElement.style.fontSize = `${innerWidth / 20}px`;
		}
	};
</script>