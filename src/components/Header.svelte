<script>
	import { page } from '$app/stores';
</script>

<header class="headerContainer">
	<nav class="navbar glass-container">
		<a href="/" class="link" class:active={$page.url.pathname === '/'}>Home</a>
		<a href="/about" class="link" class:active={$page.url.pathname === '/about'}>Sobre</a>
		<a href="/project" class="link" class:active={$page.url.pathname === '/project'}>Projetos</a>
	</nav>
</header>

<style>
	.headerContainer {
		position: fixed;
		z-index: var(--z-50);
		top: 35px;
		left: 50%;
		transform: translate(-50%, -50%);

		display: flex;
		justify-content: center;
		align-items: center;
		min-height: 75px;
	}

	.navbar {
		display: flex;
		gap: var(--spacing-12);
		padding: var(--spacing-3) var(--spacing-16);
		margin: 0px auto;
	}

	.link {
		font-size: 1.3rem;

		color: var(--color-primary);
		text-decoration: none;
	}
	.active {
		transition: 0.3s;
		color: var(--color-secondary);
	}
</style>
