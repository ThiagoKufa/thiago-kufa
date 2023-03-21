<script lang="ts">
</script>

<svelte:head>
	<title>Thiago Kufa | Sobre</title>
	<meta name="description" content="Projetos de Thiago Kufa" />
</svelte:head>

<main>
	<div class="desciption-wrap glass-container">
		<img
			src="https://media.licdn.com/dms/image/D4D16AQEtMzJHkRKOlg/profile-displaybackgroundimage-shrink_350_1400/0/1666609874721?e=1684972800&v=beta&t=ibb6I210-NijBY73gfPWk-FLkerc2QxuL3mtTQC4u8Q"
			alt=""
		/>
		<section>
			<h1>Eu sou Thiago de Paula Kufa,</h1>
			<p>
				um desenvolvedor Full-Stack pleno com mais de 5 anos de experiência em projetos. Possuo
				habilidades em liderança de equipe, desenvolvimento de aplicações web responsivas e
				otimização de performance.
			</p>
			<p>
				Minha experiência inclui liderança técnica de equipe de 5 desenvolvedores front-end,
				desenvolvimento de aplicações web responsivas utilizando React e Redux, otimização de
				performance e melhoria de UX/UI, e implementação de testes automatizados utilizando Jest.
			</p>
			<p>
				Eu possuo conhecimentos em diversas linguagens de programação, frameworks e bibliotecas,
				ferramentas de desenvolvimento e metodologias ágeis. Além disso, tenho formação acadêmica em
				Análise e Desenvolvimento de Sistemas, e já participei de especializações técnicas em
				Flutter, TDD, Clean Architecture, SOLID e Design Patterns, e NodeJs, Typescript, TDD, DDD,
				Clean Architecture e SOLID.
			</p>
			<p>
				Estou à procura de novas oportunidades e acredito que posso contribuir significativamente
				para sua organização. Por favor, não hesite em entrar em contato comigo se você tiver alguma
				oportunidade disponível.
			</p>
			<div class="att">
				<p>Atenciosamente, Thiago de Paula Kufa</p>
			</div>
		</section>
	</div>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin: 20px;
	}
	.desciption-wrap {
		display: flex;
		flex-direction: column;
		max-width: var(--screens-md);
	}
	.desciption-wrap section {
		padding: var(--spacing-10);
	}
	.att {
		margin-top: var(--spacing-15);
		align-self: flex-end;
	}
	@media only screen and (max-width: 956px) {
		.desciption-wrap {
			max-width: 100vw;
			max-width: 100dvw;
			width: 95%;
		}
	}
</style>
