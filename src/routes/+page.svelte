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
	<div class="hero__content svg-img">
		<HeroImage />
	</div>
</header>

<style>
	.hero {
		display: flex;

		padding: 0 var(--spacing-10);
		gap: var(--spacing-10);
	}
	.hero__content {
		display: flex;

		justify-content: center;
		align-items: center;
	}
	.description-wrap {
		display: flex;
		flex-direction: column;
		width: 95%;
		max-width: 500px;
		padding: var(--spacing-10);
		padding-bottom: 0;
	}
	.description-wrap h3 {
		font-size: 32px;
	}
	.description-wrap h3 span {
		color: var(--color-primary);
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
		border: 2px solid var(--color-primary);
		border-radius: 50%;
		font-size: 24px;
		color: var(--color-primary);
		text-decoration: none;
		margin: 30px 15px 30px 0px;
		transition: 0.5s ease;
	}
	.description-wrap__social-media a:hover {
		background-color: var(--color-primary);
		color: #38556d;
		box-shadow: 0 0 20px var(--color-primary);
	}

	@media only screen and (max-width: 956px) {
		.hero {
			flex-direction: column-reverse;
			justify-content: flex-end;

			gap: 0;
			padding: 5px;
			min-height: 100vh;
			min-height: 100dvh;
		}
		.hero__content {
			flex: none;
		}
		.hero__content h1 {
			font-size: 2rem;
		}
		.hero__content h3 {
			font-size: 1.5rem;
		}
		.description-wrap {
			width: auto;
		}
		.svg-img {
			width: 95vw;
			padding: 0;
			display: 0;
		}
	}
</style>
