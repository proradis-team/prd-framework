# Typography

## Headers
```html
/*vue*/
<template>
    <div id="demo-headers">
        <element class='wrapper' :is="header">
					Speak of the devil, and he shall appear.
				</element>
				
				<br>

				<b>Available options</b>
				<div class="d-grid">
					<div class="input">
						<input type="radio" id="header-h1" value="h1" v-model="header">
						<label for="header-h1">&lt;h1&gt;</label>
					</div>
					<div class="input">
						<input type="radio" id="header-h2" value="h2" v-model="header">
						<label for="header-h2">&lt;h2&gt;</label>
					</div>
					<div class="input">
						<input type="radio" id="header-h3" value="h3" v-model="header">
						<label for="header-h3">&lt;h3&gt;</label>
					</div>
					<div class="input">
						<input type="radio" id="header-h4" value="h4" v-model="header">
						<label for="header-h4">&lt;h4&gt;</label>
					</div>
					<div class="input">
						<input type="radio" id="header-h5" value="h5" v-model="header">
						<label for="header-h5">&lt;h5&gt;</label>
					</div>
					<div class="input">
						<input type="radio" id="header-h6" value="h6" v-model="header">
						<label for="header-h6">&lt;h6&gt;</label>
					</div>
				</div>
    </div>
</template>

<script>
	export default {
		data() {
			return {
				header: 'h1'
			}
		}
	}
</script>

<style>
#demo-headers .d-grid {
	grid-template-columns: 25% 25% 25% 25%;
}
</style>
```

## Alignment and Decorations


```html
/*vue*/
<template>
    <div id="demo-text">
        <div class='wrapper' :class="textClass">
					Someone like you. Someone who'll rattle the cages.
				</div>
				
				<br>

				<b>Available options</b>
				<div class="d-grid">
					<div class="input">
						<input type="radio" id="text-left" value="text-left" v-model="textClass">
						<label for="text-left">.text-left</label>
					</div>
					<div class="input">
						<input type="radio" id="text-center" value="text-center" v-model="textClass">
						<label for="text-center">.text-center</label>
					</div>
					<div class="input">
						<input type="radio" id="text-right" value="text-right" v-model="textClass">
						<label for="text-right">.text-right</label>
					</div>
					<div class="input">
						<input type="radio" id="text-underline" value="text-underline" v-model="textClass">
						<label for="text-underline">.text-underline</label>
					</div>
					<div class="input">
						<input type="radio" id="text-truncate" value="text-truncate w-120" v-model="textClass">
						<label for="text-truncate">.text-truncate</label>
					</div>
				</div>
    </div>
</template>

<script>
	export default {
		data() {
			return {
				textClass: 'text-left'
			}
		}
	}
</script>

<style>
#demo-text .d-grid {
	grid-template-columns: 25% 25% 25% 25%;
}

#demo-text .w-120 {
	width:120px;
}
</style>
```