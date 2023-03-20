<!-- src/App.svelte -->
<script>
</script>

<div class="box">
	<div class="right-effects" />
	<div class="left-effects" />
</div>

<style>
	.box {
		position: relative;
		z-index: 1;
	}
	.right-effects {
		position: fixed;
		top: 50px;
		right: 0;
		bottom: auto;
		width: 500px;
		height: 500px;
		border-radius: 50%;
		background: #f64f59;
		-webkit-filter: blur(100px);
		filter: blur(100px);
		opacity: 0.25;
		pointer-events: none;
		z-index: -1;
	}
	.left-effects {
		position: fixed;
		bottom: 50px;
		left: 0;
		width: 500px;
		height: 500px;
		border-radius: 50%;
		background: #c471ed;
		-webkit-filter: blur(100px);
		filter: blur(100px);
		opacity: 0.25;
		pointer-events: none;
		z-index: -1;
	}
</style>
