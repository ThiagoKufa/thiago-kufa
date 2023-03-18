<script>
	import heroImage from '../lib/images/programmer.svg';
</script>

<header class="hero">
	<div class="hero__content">
		<div>
			<div class="line" />
			<h1>Olá, Sou Thiago Kufa</h1>
			<h4>Desenvolvedor Full stack</h4>
			<p>Procura construir seu app e expandir seu negócio? Vamos trabalhar juntos!</p>
		</div>
	</div>
	<div class="hero__content">
		<img class="hero__content__img" src={heroImage} alt="ilustração" />
	</div>
</header>

<style>
	.hero {
		display: flex;
		padding: 0 var(--spacing-10);
		gap: var(--spacing-10);
		height: var(--screens-sm);
	}
	.hero__content {
		display: flex;
		flex: 1;
		justify-content: center;
		align-items: center;
		/* border: 1px solid var(--color-primary); */
	}
	.line {
		border: 1px solid var(--color-danger);
		width: var(--spacing-15);
		margin-bottom: var(--spacing-6);
	}
	.hero__content__img {
		width: 600px;
	}
</style>
