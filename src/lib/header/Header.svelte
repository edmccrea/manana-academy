<script lang="ts">
	import { page } from '$app/stores';
</script>

<nav>
	<a class="logo" href="/">Mañana</a>

	<ul data-sveltekit-prefetch class="desktop-nav">
		<li>
			<a href="/classes" class:active={$page.url.pathname === '/classes'} class="nav-link"
				>Classes</a
			>
		</li>
		<li>
			<a href="/timetable" class:active={$page.url.pathname === '/timetable'} class="nav-link"
				>Timetable</a
			>
		</li>
		<li>
			<a href="/coaches" class:active={$page.url.pathname === '/coaches'} class="nav-link"
				>Coaches</a
			>
		</li>
		<li>
			<a href="/about" class:active={$page.url.pathname === '/about'} class="nav-link">About</a>
		</li>
		<li>
			<a href="/blog" class:active={$page.url.pathname === '/blog'} class="nav-link">Blog</a>
		</li>
	</ul>
</nav>

<style>
	nav {
		position: sticky;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 2rem;
		height: 70px;
		border-bottom: 1px solid rgba(0, 0, 0, 0.157);
	}

	.logo {
		padding-left: 2rem;
	}

	.desktop-nav {
		display: none;
		justify-content: center;
		align-items: center;
	}

	nav li {
		margin: 0 1rem;
	}

	nav a {
		color: black;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	.nav-link::after {
		transition: all ease-in-out 300ms;
		background: none repeat scroll 0 0 black;
		content: '';
		display: block;
		height: 2px;
		width: 0;
	}

	.nav-link:hover:after {
		width: 100%;
	}

	nav a.active {
		border-bottom: 2px solid black;
	}

	a:hover {
		color: var(--tertiary-color);
	}

	@media (min-width: 768px) {
		.desktop-nav {
			display: flex;
		}
	}
</style>
