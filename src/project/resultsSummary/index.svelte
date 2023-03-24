<svelte:head>
	<link
		href="https://fonts.googleapis.com/css2?family=Caveat&family=Hanken+Grotesk:wght@500;700;800&family=Open+Sans:wght@300&display=swap"
		rel="stylesheet"
	/>
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
	/* 
# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

## Colors

### Primary

- Light red: hsl(0, 100%, 67%)
- Orangey yellow: hsl(39, 100%, 56%)
- Green teal: hsl(166, 100%, 37%)
- Cobalt blue: hsl(234, 85%, 45%)

## Gradients

- Light slate blue (background): hsl(252, 100%, 67%)
- Light royal blue (background): hsl(241, 81%, 54%)

- Violet blue (circle): hsla(256, 72%, 46%, 1)
- Persian blue (circle): hsla(241, 72%, 46%, 0)



### Neutral

- White: hsl(0, 0%, 100%)
- Pale blue: hsl(221, 100%, 96%)
- Light lavender: hsl(241, 100%, 89%)
- Dark gray blue: hsl(224, 30%, 27%)

### Notes

Use transparency to get the colour variations
necessary to match the design. Hint: look into
using `hsla()`.

## Typography

### Body Copy

- Font size (paragraphs): 18px

### Font

- Family: [Hanken Grotesk](https://fonts.google.com/specimen/Hanken+Grotesk)
- Weights: 500, 700, 800
   */
</style>
