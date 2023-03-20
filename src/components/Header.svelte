<script>
	import { page } from '$app/stores';
</script>

<header class="headerContainer">
	<nav class="navbar">
		<a href="/" class="link" class:active={$page.url.pathname === '/'}>Home</a>
		<a href="/about" class="link" class:active={$page.url.pathname === '/about'}>Sobre</a>
		<a href="/contact" class="link" class:active={$page.url.pathname === '/contact'}>Contato</a>
	</nav>
</header>

<style>
	.headerContainer {
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
		background: linear-gradient(75deg, rgba(2, 0, 48, 0.1) 0%, rgba(255, 255, 255, 0.01) 100%);
		backdrop-filter: blur(5px);
		border-radius: 20px;
		border-bottom: 1px solid rgba(0, 0, 0, 0.4);
		border-top: 1px solid rgba(80, 129, 185, 0.2);
		box-shadow: 0px 10px 10px rgba(0, 0, 0, 0.5);
	}

	.link {
		font-size: 1.3rem;

		color: var(--color-primary);
		text-decoration: none;
	}
	.active {
		transition: 0.3s;
		color: var(--color-danger);
	}
</style>
