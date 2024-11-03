<script>
	import Integrations from "./assets/Integrations.svelte";
	import LandingPage from "./assets/LandingPage.svelte";
	import Developer from "./assets/Developer.svelte";
</script>

<section class="container section-spacing services">
	<header class="header-margin">
		<h2 id="services">Empowering Your Digital Presence</h2>
		<p>
			At Donohoo Dev, we offer a comprehensive range of services to help businesses establish
			a strong digital presence and achieve their goals. Our expertise spans full-stack
			development, e-commerce solutions, internal tools, and performance optimization.
		</p>
	</header>

	<div class="service-sections">
		<div class="service">
			<div class="description">
				<h3>Full-Stack Development</h3>
				<p>
					Our skilled team of developers specializes in crafting robust, scalable web
					applications tailored to your unique requirements. From front-end design to
					back-end architecture, we leverage cutting-edge technologies to deliver
					seamless, high-performance solutions that engage users and drive results.
				</p>
			</div>

			<Developer />
		</div>

		<div class="service">
			<div class="description">
				<h3>Landing Pages with SEO & Speed Optimization</h3>
				<p>
					We create stunning, conversion-focused landing pages that captivate your
					audience and drive action. Our team optimizes your pages for search engines,
					ensuring maximum visibility and organic traffic. Plus, we prioritize speed and
					performance, delivering lightning-fast experiences that keep visitors engaged
					and boost conversions.
				</p>
			</div>

			<LandingPage />
		</div>

		<div class="service">
			<div class="description">
				<h3>Internal Tools & Integrations</h3>
				<p>
					We develop custom internal tools that streamline your workflows, automate tasks,
					and enhance productivity. Whether you need a powerful CMS or a robust e-commerce
					platform, we've got you covered. Our solutions are tailored to your unique
					needs, ensuring seamless integration and maximum efficiency.
				</p>
			</div>

			<Integrations />
		</div>
	</div>
</section>

<style scoped>
	.service-sections {
		display: grid;
		gap: 4rem;

		@media (min-width: 768px) {
		}

		@media (min-width: 1024px) {
			gap: 8rem;
		}

		& > .service {
			display: grid;
			justify-items: center;

			@media (min-width: 768px) {
				grid-template-columns: 1fr 1fr;
				align-items: center;
				column-gap: 4rem;

				&:not(:last-child) {
					margin-bottom: 4rem;
				}
			}

			@media (min-width: 1024px) {
				column-gap: 8rem;
			}

			& > svg {
				transform: scale(1.125);
			}

			@media (min-width: 768px) {
				&:nth-child(even) {
					& > .description {
						grid-row: 2;
						grid-column: 2;
					}

					& > svg {
						grid-row: 2;
						grid-column: 1;
					}
				}
			}
		}
	}
</style>
