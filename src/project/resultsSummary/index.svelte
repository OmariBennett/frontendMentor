<svelte:head>
	<link rel="stylesheet" />
	<title>Frontend Mentor | Results summary component</title>
</svelte:head>

<h1>Frontend Mentor | Results Summary Component</h1>
<main>
	<section>
		<h2>Your Result</h2>
		<p><span>76</span> of 100</p>
		<span>Great</span>
		<p>
			You scored higher than 65% of the people who have taken these tests.<br />
			Summary
		</p>
		<ul>
			<li>Reaction 80 / 100</li>
			<li>Memory 92 / 100</li>
			<li>Verbal 61 / 100</li>
			<li>Visual 72 / 100</li>
		</ul>
		<input type="button" value="Continue" />
	</section>
</main>

<div class="attribution">
	Challenge by
	<a href="https://www.frontendmentor.io?ref=challenge" target="_blank"
		>Frontend Mentor</a
	>. Coded by <a href="#">Your Name Here</a>.
</div>

<style>
	/* The designs were created to the following widths: */
	/* - Mobile: 375px */
	/* - Desktop: 1440px */
	main {
		/* ## Colors */
		/* ### Primary */
		--accent-color-1: hsl(0, 100%, 67%); /* Light red */
		--accent-color-2: hsl(39, 100%, 56%); /* Orangey yellow */
		--accent-color-3: hsl(166, 100%, 37%); /* Green teal */
		--accent-color-4: hsl(234, 85%, 45%); /* Cobalt blue */

		/* ## Gradients */
		/* Light slate blue (background) to Light royal blue (background) */
		--gradient-1: hsl(252, 100%, 67%), hsl(252, 100%, 67%);
		/* Violet blue (circle) to Persian blue (circle) */
		--gradient-2: hsla(256, 72%, 46%, 1), hsla(241, 72%, 46%, 0);

		/* ### Neutral */
		--neutral-hsl-color-100: hsl(0, 0%, 100%); /* White */
		--neutral-hsl-color-200: hsl(221, 100%, 96%); /* Pale blue */
		--neutral-hsl-color-400: hsl(241, 100%, 89%); /* Light lavender */
		--neutral-hsl-color-900: hsl(224, 30%, 27%); /* Dark gray blue */

		/* ## Typography */
		/* - Family: [Hanken Grotesk](https://fonts.google.com/specimen/Hanken+Grotesk) */
		/* - Weights: 500, 700, 800 */
		@font-face {
			font-family: 'Hanken Grotesk';
			font-display: swap;
			font-weight: 100 900;
			src: local('Hanken Grotesk'),
				url('../../../projects/results-summary-component-main/assets/fonts/HankenGrotesk-VariableFont_wght.ttf')
					format('TrueType'),
				url('https://fonts.googleapis.com/css2?family=Caveat&family=Hanken+Grotesk:wght@500;700;800&family=Open+Sans:wght@300&display=swap')
					format('TrueType');
		}
	}
	:global(body) {
		font-size: 1.125rem; /* - Font size (paragraphs): 18px */
		font-family: 'Hanken Grotesk';
	}
</style>
