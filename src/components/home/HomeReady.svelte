<script>
	import ButtonLink from "$components/common/ButtonLink.svelte";
	import Astronaut from "./assets/Astronaut.svelte";
</script>

<section class="container section-spacing ready">
	<header class="header-margin">
		<h2 id="ready">Ready to take your business to the next level?</h2>
		<p>
			Take the next step in your digital journey with Donohoo Dev. Our team of experts is here
			to help you unlock your website's full potential and drive your business forward.
			Whether you're looking to boost performance, enhance user experience, or improve your
			online visibility, we have the solutions you need to succeed.
		</p>
	</header>

	<Astronaut />
	<ButtonLink variant="primary" size="lg" href="/contact">Launch</ButtonLink>
</section>

<style scoped>
	.ready {
		display: grid;
		justify-items: center;
		text-align: center;
		gap: 4rem;

		& > header {
			margin-bottom: 0;

			& > p {
				max-width: 65ch;
				margin-inline: auto;
			}
		}
	}

	.ready > :global(svg) {
		margin-top: -4rem;
		max-width: 325px;
	}

	.ready > :global(.btn) {
		width: 100%;
		max-width: 34ch;
	}
</style>
