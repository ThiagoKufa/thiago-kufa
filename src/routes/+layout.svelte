<script>
	import Header from '$components/Header.svelte';
	import './globals.css';
</script>

<head>
	<meta
		name="description"
		content="Procura construir seu app e expandir seu negócio? Vamos trabalhar juntos!"
	/>
	<title>Thiago Kufa</title>
</head>
<div class="app">
	<Header />
	<main>
		<slot />
		<div class="right-effects" />
		<div class="left-effects" />
	</main>
	<footer>
		<div class="footer__content">
			<div class="footer__content__contact">
				<p>E-mail: tkufa.code@gmail.com</p>
				<p>Celular/WhatsApp: (11) 95791-4190</p>
				<p>
					LinkedIn: <a href="http://linkedin.com/in/thiago-kufa">linkedin.com/in/thiago-kufa</a>
				</p>
			</div>
		</div>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		position: relative;

		display: flex;
		flex: 1;
		flex-direction: column;
		justify-content: center;

		padding-top: 80px;
		width: 100%;
		min-height: 100vh;
		min-height: 100dvh;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}
	footer {
		background-color: black;
	}
	.footer__content {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: flex-end;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}
	.footer__content__contact a {
		color: var(--color-primary);
	}

	.right-effects {
		position: absolute;
		top: 50px;
		right: 0;
		bottom: auto;
		width: 500px;
		height: 500px;
		border-radius: 50%;
		background: #4fe3f6;
		-webkit-filter: blur(100px);
		filter: blur(100px);
		opacity: 0.15;
		pointer-events: none;
		z-index: -2;
	}
	.left-effects {
		position: fixed;
		bottom: 50px;
		width: 500px;
		height: 500px;
		border-radius: 50%;
		background: #c471ed;
		-webkit-filter: blur(100px);
		filter: blur(100px);
		opacity: 0.15;
		pointer-events: none;
		z-index: -2;
	}
</style>
