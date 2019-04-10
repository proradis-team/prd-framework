# Alerts and Labels
## Alerts

```html
/*vue*/
<template>
    <div id="demo-text">
        <div class='alert' :class="textClass">
					Someone like you. Someone who'll rattle the cages.
				</div>
				
				<br>

				<b>Available options</b>
				<div class="d-grid">
					<div class="input">
						<input type="radio" id="alert-danger" value="alert-danger" v-model="textClass">
						<label for="alert-danger">.alert-danger</label>
					</div>
					<div class="input">
						<input type="radio" id="alert-warning" value="alert-warning" v-model="textClass">
						<label for="alert-warning">.alert-warning</label>
					</div>
					<div class="input">
						<input type="radio" id="alert-info" value="alert-info" v-model="textClass">
						<label for="alert-info">.alert-info</label>
					</div>
					<div class="input">
						<input type="radio" id="alert-success" value="alert-success" v-model="textClass">
						<label for="alert-success">.alert-success</label>
					</div>
				</div>
    </div>
</template>

<script>
	export default {
		data() {
			return {
				textClass: 'alert-success'
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

## Labels

```html
/*vue*/
<template>
    <div id="demo-text">
        <span class='label' :class="textClass">
					Some text
				</span>
				
				<br>

				<b>Available options</b>
				<div class="d-grid">
					<div class="input">
						<input type="radio" id="label-danger" value="label-danger" v-model="textClass">
						<label for="label-danger">.label-danger</label>
					</div>
					<div class="input">
						<input type="radio" id="label-warning" value="label-warning" v-model="textClass">
						<label for="label-warning">.label-warning</label>
					</div>
					<div class="input">
						<input type="radio" id="label-info" value="label-info" v-model="textClass">
						<label for="label-info">.label-info</label>
					</div>
					<div class="input">
						<input type="radio" id="label-success" value="label-success" v-model="textClass">
						<label for="label-success">.label-success</label>
					</div>
				</div>
    </div>
</template>

<script>
	export default {
		data() {
			return {
				textClass: 'label-success'
			}
		}
	}
</script>

<style>
#demo-label .d-grid {
	grid-template-columns: 25% 25% 25% 25%;
}

#demo-label .w-120 {
	width:120px;
}
</style>
```