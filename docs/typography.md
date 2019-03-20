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
					<label><input type="radio" value="h1" v-model="header">h1</label>
					<label><input type="radio" value="h2" v-model="header">h2</label>
					<label><input type="radio" value="h3" v-model="header">h3</label>
					<label><input type="radio" value="h4" v-model="header">h4</label>
					<label><input type="radio" value="h5" v-model="header">h5</label>
					<label><input type="radio" value="h6" v-model="header">h6</label>
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
					<label><input type="radio" value="text-left" v-model="textClass"> .text-left</label>
					<label><input type="radio" value="text-center" v-model="textClass"> .text-center</label>
					<label><input type="radio" value="text-right" v-model="textClass"> .text-right</label>
					<label><input type="radio" value="text-underline" v-model="textClass"> .text-underline</label>
					<label><input type="radio" value="text-truncate w-120" v-model="textClass"> .text-truncate</label>
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