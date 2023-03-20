<script lang="ts">
</script>

<svelte:head>
	<title>Projetos</title>
	<meta name="description" content="Projetos de Thiago Kufa" />
</svelte:head>
<header>
	<h1>Thiago de Paula Kufa</h1>
</header>
<main>
	<section>
		<h2>Sobre Mim</h2>
		<p>
			Eu sou um desenvolvedor front-end com mais de 5 anos de experiência em projetos de grande
			porte. Tenho experiência em liderança de equipe, desenvolvimento de aplicações web responsivas
			e otimização de performance.
		</p>
	</section>
	<section>
		<h2>Experiência</h2>
		<ul>
			<li>
				<h3>Desenvolvedor Front-End Pleno na Arteprog</h3>
				<p>Jan de 2016 - Nov de 2021</p>
				<ul>
					<li>Liderança técnica de equipe de 5 desenvolvedores front-end</li>
					<li>Desenvolvimento de aplicações web responsivas utilizando React e Redux</li>
					<li>Otimização de performance e melhoria de UX/UI</li>
					<li>Implementação de testes automatizados utilizando Jest</li>
				</ul>
			</li>
			<li>
				<h3>Desenvolvedor Front-End Pleno na Digital Pages</h3>
				<p>Jan de 2022 - Out de 2022</p>
				<ul>
					<li>Desenvolvimento de soluções web responsivas utilizando React e Next.js</li>
					<li>Manutenção de projetos legados e refatoração de código</li>
					<li>Participação em projetos de grande porte</li>
				</ul>
			</li>
			<li>
				<h3>Desenvolvedor Front-End Júnior na Grid Service</h3>
				<p>Mar de 2015 - Jan de 2016</p>
				<ul>
					<li>Desenvolvimento de soluções web utilizando HTML, CSS e JavaScript</li>
					<li>Participação em projetos de pequeno porte</li>
					<li>Aprendizado de frameworks e bibliotecas como React</li>
				</ul>
			</li>
		</ul>
	</section>
	<section>
		<h2>Educação</h2>
		<ul>
			<li>
				<h3>Análise e Desenvolvimento de Sistemas na Estácio</h3>
				<p>2018-2020</p>
			</li>
		</ul>
		<h2>Especialização Técnica</h2>
		<ul>
			<li>
				<h3>Flutter, TDD, Clean Architecture, SOLID e Design Patterns com Rodrigo Manguinho</h3>
				<p>2021-2022</p>
			</li>
			<li>
				<h3>NodeJs, Typescript, TDD, DDD, Clean Architecture e SOLID com Rodrigo Manguinho</h3>
				<p>2021-2022</p>
			</li>
		</ul>
	</section>
</main>

<style>
	header {
		color: #fafafa;
		display: flex;
		justify-content: space-between;
		padding: 10px;
	}

	main {
		margin: 20px;
	}

	section {
		margin-bottom: 40px;
	}

	h2 {
		font-size: 24px;
		margin-bottom: 10px;
	}

	ul {
		list-style: none;
		margin: 0;
		padding: 0;
	}

	h3 {
		font-size: 20px;
		margin-bottom: 5px;
	}
</style>
