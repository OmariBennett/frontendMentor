<svelte:head>
	<link rel="stylesheet" />
	<title>Frontend Mentor &#124; Results summary component</title>
</svelte:head>

<div class="background">
	<h1 class="heading-0">
		Frontend Mentor <span>&#124;</span> Results Summary Component
	</h1>
	<main>
		<section class="result | text-align-center ">
			<div class="summary | grid align-center" data-gap="large">
				<h2 class="heading-1">Your Result</h2>
				<p><span>76</span> of 100</p>
				<div>
					<p>Great</p>
					<p>
						You scored higher than 65% of the people who have taken these tests.
					</p>
				</div>
			</div>

			<div class="detail">
				<p class="heading-1">Summary</p>
				<ul>
					<li>Reaction 80 / 100</li>
					<li>Memory 92 / 100</li>
					<li>Verbal 61 / 100</li>
					<li>Visual 72 / 100</li>
				</ul>
				<input type="button" value="Continue" />
			</div>
		</section>
	</main>

	<div class="attribution">
		Challenge by
		<a href="https://www.frontendmentor.io?ref=challenge" target="_blank"
			>Frontend Mentor</a
		>. Coded by <a href="#customLinkNeeded">Your Name Here</a>.
	</div>
</div>

<style>
	/* The designs were created to the following widths: */
	/* - Mobile: 375px equal to 23em*/
	/* - Desktop: 1440px equal to 90em*/
	/* Table of Content
	# Setup
	# Component
	# Utility
	# Block
	# Exception
	# Other
	*/

	/***************************************
	 * SETUP
	 ****************************************/
	/* ## Typography */
	/* - Family: [Hanken Grotesk](https://fonts.google.com/specimen/Hanken+Grotesk) */
	/* - Weights: 500, 700, 800 */
	:root {
		--accent-hsl-color-1: 0 100% 67%; /* Light red */
		--accent-hsl-color-2: 39 100% 56%; /* Orangey yellow */
		--accent-hsl-color-3: 166 100% 37%; /* Green teal */
		--accent-hsl-color-4: 234 85% 45%; /* Cobalt blue */

		--accent-color-1: hsl(var(--accent-hsl-color-1));
		--accent-color-2: hsl(var(--accent-hsl-color-2));
		--accent-color-3: hsl(var(--accent-hsl-color-3));
		--accent-color-4: hsl(var(--accent-hsl-color-4));

		--neutral-hsl-color-100: 0 0% 100%; /* White */
		--neutral-hsl-color-200: 221 100% 96%; /* Pale blue */
		--neutral-hsl-color-400: 241 100% 89%; /* Light lavender */
		--neutral-hsl-color-900: 224 30% 27%; /* Dark gray blue */

		--neutral-color-100: hsl(var(--neutral-hsl-color-100));
		--neutral-color-200: hsl(var(--neutral-hsl-color-200));
		--neutral-color-400: hsl(var(--neutral-hsl-color-400));
		--neutral-color-900: hsl(var(--neutral-hsl-color-900));

		/* ## Gradients */
		/* Light slate blue (background) to Light royal blue (background) */
		--gradient-1: hsl(252, 100%, 67%), hsl(241, 81%, 54%);
		/* Violet blue (circle) to Persian blue (circle) */
		--gradient-2: hsla(256, 72%, 46%, 1), hsla(241, 72%, 46%, 0);

		/* - Weights: 500, 700, 800 */
		--regular: 500;
		--semi-bold: 700;
		--bold: 800;

		--clr: hsl(0, 100%, 67%); /* Light red */
		--clr: hsl(39, 100%, 56%); /* Orangey yellow */
		--clr: hsl(166, 100%, 37%); /* Green teal */
		--clr: hsl(234, 85%, 45%); /* Cobalt blue */
		--clr: hsl(252, 100%, 67%); /* Light slate blue (background) */
		--clr: hsl(252, 100%, 67%); /* Light royal blue (background) */
		--clr: hsla(256, 72%, 46%, 1); /* Violet blue (circle) */
		--clr: hsla(241, 72%, 46%, 0); /* Persian blue (circle) */
		--clr: hsl(0, 0%, 100%); /* White */
		--clr: hsl(221, 100%, 96%); /* Pale blue */
		--clr: hsl(241, 100%, 89%); /* Light lavender */
		--clr: hsl(224, 30%, 27%); /* Dark gray blue */
	}
	@font-face {
		font-family: 'Hanken Grotesk';
		font-display: swap;
		font-weight: 100 900;
		src: local('Hanken Grotesk'),
			url('../../public/results-summary-component-main/assets/fonts/HankenGrotesk-VariableFont_wght.ttf')
				format('TrueType');
	}
	* {
		font: inherit;
		outline: 1px solid indigo;
		/* background-color: hsl(275 100% 25% / 0.1); */
	}
	:global(html, body, #app),
	main {
		min-height: 100vh;
	}
	:global(body) {
		letter-spacing: 1.1px;
		line-height: 1.6;
		font-family: 'Hanken Grotesk';
		font-size: 1.125rem; /* - Font size (paragraphs): 18px */
		font-weight: var(--regular);
		color: var(--neutral-color-900);
	}
	@media (min-width: 23em) {
		main {
			place-items: center;
		}
	}
	/***************************************
	 * Component
	 ****************************************/

	.result span {
		color: var(--neutral-color-100);
		font-size: 3rem;
		display: block;
	}
	.summary {
		color: hsl(var(--neutral-hsl-color-200) / 0.7);
		background-image: linear-gradient(var(--gradient-1));
		padding: 2rem;
		border-radius: 0 0 2rem 2rem;
	}
	.summary h2 + p:first-of-type {
		color: hsl(var(--neutral-hsl-color-200) / 0.6);
		background-color: deeppink;
		aspect-ratio: 1/1;
		border-radius: 50%;
		width: 10rem;
	}
	/***************************************
	 * Utility
	 ****************************************/
	.text-align-center {
		text-align: center;
	}
	.grid {
		display: grid;
	}
	.align-center {
		place-items: center;
	}
	[data-gap='large'] {
		gap: 2rem; /* fix the amount */
	}
	/***************************************
	 * Block
	 ****************************************/
	.heading-0 {
		font-size: 2rem;
		line-height: 0.9;
		font-weight: var(--bold);
	}
	.heading-1 {
		font-size: 1.3rem;
	}
	/***************************************
	 * Exception
	 ****************************************/
	/***************************************
	 ** OTHER
	 ****************************************/
	h1,
	.detail,
	.attribution {
		display: none;
	}
</style>
