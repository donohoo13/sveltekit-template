<script lang="ts">
	import ButtonLink from "$components/common/ButtonLink.svelte";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="" />
	<meta property="og:title" content="" />
	<meta property="og:description" content="" />
	<meta name="og:url" content="https://www." />
	<meta name="twitter:title" content="" />
	<meta name="twitter:description" content="" />
	<meta name="twitter:url" content="https://www." />
	<meta name="keywords" content="" />
</svelte:head>

<section class="container section-spacing">
	<header>
		<h1 id="welcome">Welcome to SvelteKit Template</h1>
		<p class="subtitle">Built with SvelteKit, CSS and Vite.</p>
		<ButtonLink class="test" href="/about">Learn More</ButtonLink>
	</header>
</section>

<style scoped>
	#welcome {
		color: var(--clr-text);
	}
</style>
