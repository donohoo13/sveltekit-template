<script lang="ts">
	import { goto } from "$app/navigation";
	import Button from "$components/common/Button.svelte";
	import LogoSolid from "$components/navbar/NavbarLogo.svelte";
</script>

<footer class="full-width-container main-footer">
	<div class="container">
		<div class="logo-section">
			<LogoSolid height={36} />
			<p class="catch-phrase"><em>Slogan</em></p>
		</div>

		<div class="contact">
			<p>Call to action</p>
			<Button
				class="contact-btn"
				variant="outlined"
				size="sm"
				clickHandler={() => goto("/contact")}>Contact</Button
			>
		</div>

		<div class="navigation">
			<p>Navigation</p>
			<ul>
				<li>
					<a href="/">Home</a>
				</li>
				<li>
					<a href="/">Contact</a>
				</li>
			</ul>
		</div>

		<div class="actions">
			<ul>
				<li>
					<a href="https://www.linkedin.com" target="_blank" rel="noopener noreferrer">
						<i class="fa-brands fa-linkedin-in fa-xl" />
						<span class="visually-hidden">Donohoo Dev, LLC LinkedIn profile</span>
					</a>
				</li>
				<li>
					<a rel="noopener noreferrer" target="_blank" href="https://x.com">
						<i class="fa-brands fa-x-twitter fa-xl" />
						<span class="visually-hidden">Donohoo Dev, LLC X profile</span>
					</a>
				</li>
				<li>
					<a href="https://github.com" target="_blank" rel="noopener noreferrer">
						<i class="fa-brands fa-github fa-xl" />
						<span class="visually-hidden">Donohoo Dev, LLC Github profile</span>
					</a>
				</li>
			</ul>
		</div>

		<div class="copyright">
			<ul class="links">
				<li>
					<a href="/terms-of-use">Terms of Use</a>
				</li>
				<li>
					<a href="/privacy-policy">Privacy Policy</a>
				</li>
			</ul>

			<small>
				&copy; {new Date().getFullYear()} Donohoo Development, LLC. All rights reserved.
			</small>
			<!-- ---- Attribution ---- -->
			<!-- <small class="attribution">
				Vectors designed by
				<a
					href="https://www.freepik.com/author/stories"
					title="Storyset"
					target="_blank"
					rel="noopener noreferrer"
				>
					Storyset
				</a>
			</small> -->
		</div>
	</div>
</footer>

<style scoped>
	.main-footer {
		background-color: var(--clr-primary-dark);
		color: var(--clr-white);
		padding: 4rem 2rem;

		& p {
			margin: 0;
		}

		& > .container {
			display: grid;
			gap: 4rem;

			@media (min-width: 768px) {
				grid-template-columns: 1fr 1fr;
			}
		}
	}

	.logo-section {
		@media (min-width: 768px) {
			grid-column: 1/-1;
			order: 1;
		}
	}

	.contact {
		@media (min-width: 768px) {
			grid-column: 1;
			order: 2;
		}
	}

	.contact > :global(.contact-btn) {
		width: 100%;
		max-width: 38ch;
		color: var(--clr-secondary);
		border-color: var(--clr-secondary);
		margin-top: 1rem;

		&:hover {
			background-color: var(--clr-secondary);
		}

		@media (min-width: 768px) {
			max-width: 42ch;
		}
	}

	.navigation {
		display: none;
		font-size: var(--font-size-sm);

		& > p {
			margin: 0 0 0.5rem;
			text-decoration: underline;
			margin-bottom: 2rem;
		}

		& > ul {
			display: flex;
			flex-direction: column;
			gap: 1rem;
			margin: 0;

			& > li {
				& > a {
					color: var(--clr-white);

					&:hover {
						text-decoration: underline;
					}
				}
			}
		}

		@media (min-width: 768px) {
			display: block;
			grid-column: 2;
			order: 3;
			justify-self: flex-end;
		}
	}

	.actions {
		& > ul {
			display: flex;
			gap: 2rem;
			margin: 0;
			padding: 0;

			& > li {
				& > a {
					color: var(--clr-secondary);

					&:hover {
						color: var(--clr-accent);
					}
				}
			}
		}

		@media (min-width: 768px) {
			grid-column: 2;
			order: 5;
			align-self: flex-end;
			justify-self: flex-end;
		}
	}

	.copyright {
		& > .links {
			display: flex;
			gap: 4rem;
			margin: 0 0 1rem;

			& > li {
				& > a {
					margin: 0;
					font-size: var(--font-size-sm);
					color: var(--clr-white);

					&:hover {
						text-decoration: underline;
					}
				}
			}
		}

		& > small {
			display: block;
			font-size: var(--font-size-caption);
			color: var(--clr-gray);

			&:first-of-type {
				margin-top: 2rem;
				margin-bottom: 1rem;
			}
		}

		@media (min-width: 768px) {
			grid-column: 1;
			order: 4;
		}
	}
</style>
