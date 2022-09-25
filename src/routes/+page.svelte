<script lang="ts">
</script>

<svelte:head>
	<title>Mañana Academy Ystad</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="hero">
	<h1>Manana Academy</h1>
</section>

<section class="about landing-section" data-sveltekit-prefetch>
	<h2>About Mañana</h2>
	<p>
		Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ducimus, ipsa. Ducimus, officiis? Ut,
		officia autem quasi officiis fuga doloribus nesciunt delectus alias sapiente quia minus minima
		quisquam fugiat quas quae veritatis porro facere sed. Delectus accusantium ratione pariatur sit
		ipsam. In saepe laboriosam laudantium, molestiae aliquid nemo voluptatibus consequat <a
			href="/about"
			class="more-link">read more...</a
		>
	</p>
</section>

<section class="instagram-feed" />
<section class="external-links" />

<style>
	.hero {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	.landing-section {
		max-width: 786px;
		margin: 1rem auto;
	}

	h1 {
		width: 100%;
	}

	.more-link {
		color: var(--tertiary-color);
	}
</style>
