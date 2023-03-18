<script>
	import { page } from '$app/stores';
</script>

<header class="headerContainer">
	<nav class="navbar">
		<a href="/" class="link" class:active={$page.url.pathname === '/'}>Home</a>
		<a href="/projects" class="link" class:active={$page.url.pathname === '/projects'}>Projetos</a>
		<a href="/contact" class="link" class:active={$page.url.pathname === '/contact'}>Contato</a>
	</nav>
</header>

<style>
	.headerContainer {
		display: flex;
		justify-content: center;
		border: 1px solid var(--color-primary);
	}
	.navbar {
		display: flex;
		gap: var(--spacing-12);
		padding: var(--spacing-3) var(--spacing-12);
	}

	.link {
		color: var(--color-primary);
		text-decoration: none;
	}
	.active {
		color: var(--color-danger);
	}
</style>
