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
	</main>
	<footer>
		<div class="footer__content">
			<div class="footer__content__contact">
				<p>E-mail: tkufa.code@gmail.com</p>
				<p>Celular/WhatsApp: (11) 95791-4190</p>
				<p>
					LinkedIn: <a href="<http://linkedin.com/in/thiago-kufa>">linkedin.com/in/thiago-kufa</a>
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
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}
	footer {
		border-top: 1px solid var(--color-primary);
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
</style>
