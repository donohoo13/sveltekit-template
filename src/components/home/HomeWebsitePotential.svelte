<section class="full-width-breakout-container section-spacing potential">
	<div class="container">
		<header class="header-margin">
			<h2 id="potential">Unlocking Your Website's Full Potential</h2>
			<p>At Donohoo Dev, we focus on the key elements that drive your online success.</p>
		</header>

		<ul class="focuses">
			<li class="focus">
				<i class="fa-regular fa-chart-mixed" />
				<h3>Performance Optimization</h3>
				<p>Boosting your website's speed and performance for optimal user experience.</p>
			</li>

			<li class="focus">
				<i class="fa-regular fa-gauge-circle-bolt" />
				<h3>Efficiency</h3>
				<p>Increasing your online visibility and search rankings for more traffic.</p>
			</li>

			<li class="focus">
				<i class="fa-regular fa-universal-access" />
				<h3>Accessibility</h3>
				<p>Creating inclusive websites that are usable by people of all abilities.</p>
			</li>

			<li class="focus">
				<i class="fa-regular fa-chess" />
				<h3>Strategic Development</h3>
				<p>Aligning technology with best practices to achieve your business goals.</p>
			</li>
		</ul>
	</div>
</section>

<style scoped>
	.potential {
		background-color: var(--clr-primary-dark);
		color: var(--clr-white);
	}

	.focuses {
		display: grid;
		grid-auto-rows: 1fr;
		gap: 4rem;

		@media (min-width: 480px) {
			grid-template-columns: 1fr 1fr;
		}

		@media (min-width: 768px) {
			gap: 8rem;
		}

		@media (min-width: 1080px) {
			grid-template-columns: 1fr 1fr 1fr 1fr;
			justify-content: space-between;
		}

		& svg {
			color: var(--clr-accent);
			font-size: 7rem;
		}

		& h3 {
			font-size: var(--font-size-h5);
			text-wrap: nowrap;
		}

		& p {
			font-size: 1.5rem;
		}
	}
</style>
