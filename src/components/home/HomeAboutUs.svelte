<section class="breakout-container section-spacing who-we-are">
	<header class="header-margin">
		<h2 id="innovators">Innovators at Heart</h2>
		<p>
			At Donohoo Dev, we're more than just a development company. We're a team of passionate
			innovators dedicated to transforming ideas into powerful digital solutions.
		</p>
	</header>

	<div class="who-we-are-cards">
		<div class="card">
			<i class="fa-duotone fa-solid fa-laptop-code icon" />
			<h3>Passion Meets Expertise</h3>
			<p>
				Our team combines deep technical expertise with creative problem-solving, delivering
				innovative solutions for every project.
			</p>
		</div>

		<div class="card">
			<i class="fa-duotone fa-solid fa-ear-listen icon" />
			<h3>We Hear You</h3>
			<p>
				We believe in collaboration and open communication, building strong partnerships
				that lead to successful outcomes.
			</p>
		</div>

		<div class="card">
			<i class="fa-duotone fa-solid fa-bullseye-arrow icon" />
			<h3>Driving Your Success</h3>
			<p>
				Your success is our top priority. We deliver high-quality solutions that drive your
				business forward.
			</p>
		</div>
	</div>
</section>

<style scoped>
	.who-we-are {
		background-color: hsl(from var(--clr-primary) h s l / 0.4);
		text-align: center;
		display: grid;
		/* gap: 6rem; */

		@media (min-width: 768px) {
			border-radius: 1rem;
		}

		& > header {
			margin-inline: auto;
			max-width: 70ch;
		}

		& > .who-we-are-cards {
			display: grid;
			gap: 4rem;
			grid-template-columns: 1fr;
			max-width: 50ch;
			margin-inline: auto;

			@media (min-width: 1024px) {
				max-width: none;
				padding-inline: 2rem;
				grid-template-columns: repeat(3, 1fr);
			}

			& > .card {
				background-color: var(--clr-bg);
				border-radius: 1rem;
				padding: 3rem;
				box-shadow: 0 0 1.25rem 0 hsl(from var(--clr-gray) h s l / 0.5);

				@media (min-width: 1024px) {
					text-align: left;
				}

				& > .icon {
					font-size: clamp(4rem, 8vw, 5rem);
					color: var(--clr-primary);
				}

				& > h3 {
					margin-top: 3rem;
					font-size: var(--font-size-h5);
				}

				& > p {
					color: var(--clr-text);
					margin-top: 1rem;
				}
			}
		}
	}
</style>
