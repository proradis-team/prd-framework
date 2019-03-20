# Cards

Simple, clean and easy to implement. Just use!

```html
<div class="card">
	<div class="card-container">
		<!-- Content goes here -->
	</div>
	<div class="card-actions">
		<!-- Buttons goes here -->
	</div>
</div>
```

```html
/*vue*/

<template>
	<div class="card">
		<div class="card-container">
			<p>Citizens, take control. Take control of your city!</p>
			<p>You wanna know how I got them? So I had a wife. She was beautiful, like you, who tells me I worry too much, who tells me I ought to smile more, who gambles and gets in deep with the sharks. Hey. One day they carve her face. And we have no money for surgeries. She can't take it. I just wanna see her smile again. I just want her to know that I don't care about the scars. So, I do this to myself. And you know what? She can't stand the sight of me. She leaves. Now I see the funny side. Now I'm always smiling.</p>
			<p>As Gotham's favored son you will be ideally placed to strike at the heart of criminality.</p>
			<p>Didn't you get the memo?</p>
		</div>
	</div>
</template>

<script>
export default {}
</script>

<style>
.card {
	width:100%;
	max-width: 512px;
	margin: 0 auto;
}
</style>
```