<script>
	import HeroImage from '$components/icons/HeroImage.svelte';
</script>

<svelte:head>
	<title>Thiago Kufa</title>
	<meta name="description" content="Crie aplicativos e sites" />
</svelte:head>

<header class="hero ">
	<div class="hero__content">
		<div class="description-wrap glass-container">
			<div class="description-wrap__line " />
			<h3>Olá, eu sou</h3>
			<h1>Thiago Kufa</h1>
			<h3>Desenvolvedor <span>Full stack</span></h3>
			<p>Procura construir seu app e expandir seu negócio? <br />Vamos trabalhar juntos!</p>
			<div class="description-wrap__social-media">
				<a href="https://www.linkedin.com/in/thiago-kufa/" target="_blank">
					<i class="bx bxl-linkedin-square" />
				</a>
				<a href="https://github.com/ThiagoKufa" target="_blank">
					<i class="bx bxl-github" />
				</a>
				<a
					href="https://api.whatsapp.com/send/?phone=5511957914190&text&type=phone_number&app_absent=0"
					target="_blank"
				>
					<i class="bx bxl-whatsapp" />
				</a>
			</div>
		</div>
	</div>
	<div class="hero__content">
		<HeroImage />
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
	.description-wrap {
		display: flex;
		flex-direction: column;
		padding: var(--spacing-10);
		padding-bottom: 0;
	}
	.description-wrap h3 {
		font-size: 32px;
	}
	.description-wrap h3 span {
		color: #0ef;
		font-size: 32px;
	}
	.description-wrap h3:nth-of-type(2) {
		margin-bottom: 30px;
	}
	.description-wrap h1 {
		font-size: 56px;
		font-weight: 700;
		margin: -3px 0;
	}
	.description-wrap p {
		font-size: 16px;
	}
	.description-wrap__line {
		border: 1px solid var(--color-secondary);
		width: var(--spacing-15);
		margin-bottom: var(--spacing-6);
	}
	.description-wrap__social-media a {
		display: inline-flex;
		justify-content: center;
		align-items: center;
		width: 40px;
		height: 40px;
		background-color: transparent;
		border: 2px solid #0ef;
		border-radius: 50%;
		font-size: 24px;
		color: #0ef;
		text-decoration: none;
		margin: 30px 15px 30px 0px;
		transition: 0.5s ease;
	}
	.description-wrap__social-media a:hover {
		background-color: #0ef;
		color: #38556d;
		box-shadow: 0 0 20px #0ef;
	}
</style>
