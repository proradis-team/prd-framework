# List of avaiable helpers

## Text Helpers

| CSS Class | Description |
|---|---|
| .text-center | Align text on center |
| .text-right | Align text on right |
| .text-left | Align text on left |
| .text-truncate | Add dots when text is truncate, like: My truncate tex... |
| .text-underline | Underline text  |

### Usage
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