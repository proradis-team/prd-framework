## Introduction

The layout framework uses the power of Flexible Box Module, popularly called [Flex CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox).

See the specs to build a nice UI.

## Layout and Containers

First, use the css display flex to apply flexbox.

```html
<div class="d-flex"></div>
```
There's two options available to apply the orientation

|   |   |
|---|---|
| ```.flex-row``` | Apply the horizontal orientation |
| ```.flex-column``` | Apply the verticaly orientation |

### Horizontal Orientation

```html
/*vue*/
<template>
	<div class="d-flex flex-row">
		<div class="box-item"></div>
		<div class="box-item"></div>
		<div class="box-item"></div>
	</div>
</template>

<script>
	 export default {}
</script>

<style>
.box-item {
	width: 64px;
	height: 64px;
	background: #f1f5f9;
	margin: 8px;
}
</style>
```

### Vertical Orientation

```html
/*vue*/
<template>
	<div class="d-flex flex-column">
		<div class="box-item"></div>
		<div class="box-item"></div>
		<div class="box-item"></div>
	</div>
</template>

<script>
	 export default {}
</script>

<style>
.box-item {
	width: 64px;
	height: 64px;
	background: #f1f5f9;
	margin: 8px;
}
</style>
```

### Child Alignment

```html
/*vue*/
<template>
	<div>
		<div class="d-flex" style="height: 256px; border:1px solid #f1f5f9" :class="[orientation, horizontalAlign, verticalAlign]">
			<div class="box-item"></div>
			<div class="box-item"></div>
			<div class="box-item"></div>
		</div>

		<div class="d-flex d-row">
			<div class="flex">
				<div>Layout Direction</div>
				<div class="d-flex flex-column">
					<label><input type="radio" value="flex-row" v-model="orientation"> .flex-row </label>
					<label><input type="radio" value="flex-column" v-model="orientation"> .flex-column </label>
				</div>
			</div>

			<div class="flex">
				<div>Layout Direction (horizontal)</div>
				<div class="d-flex flex-column">
					<label><input type="radio" value="" v-model="horizontalAlign"> start (default) </label>
					<label><input type="radio" value="flex-items-center" v-model="horizontalAlign"> .flex-items-center </label>
					<label><input type="radio" value="flex-items-end" v-model="horizontalAlign"> .flex-items-end </label>
					<label><input type="radio" value="flex-items-space-between" v-model="horizontalAlign"> .flex-items-space-between </label>
					<label><input type="radio" value="flex-items-space-around" v-model="horizontalAlign"> .flex-items-space-around </label>
				</div>
			</div>

			<div class="flex">
				<div>Perpendicular Direction (vertical)</div>
				<div class="d-flex flex-column">
					<label><input type="radio" value="flex-content-start" v-model="verticalAlign"> .flex-content-start </label>
					<label><input type="radio" value="flex-content-center" v-model="verticalAlign"> .flex-content-center </label>
					<label><input type="radio" value="flex-content-end" v-model="verticalAlign"> .flex-content-end </label>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	 export default {
		 data() {
			 return {
				 orientation: 'flex-row',
				 verticalAlign: 'flex-content-start',
				 horizontalAlign: 'flex-items-center'
			 }
		 }
	 }
</script>

<style>
.box-item {
	background: #f1f5f9;
	margin: 8px;
	padding:8px;
}
</style>
```

### Child Options

```html
/*vue*/
<template>
	<div>
		<div class="d-flex">
			<div class="box-item" :class="childOptions"></div>
			<div class="box-item" :class="childOptions"></div>
			<div class="box-item" :class="childOptions"></div>
		</div>

		<div class="d-flex d-row">
			<div class="flex">
				<div>Options</div>
				<div class="d-flex flex-column">
					<label><input type="radio" value="flex-column" v-model="childOptions"> None </label>
					<label><input type="radio" value="flex" v-model="childOptions"> .flex </label>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	 export default {
		 data() {
			 return {
				 childOptions: ''
			 }
		 }
	 }
</script>

<style>
.box-item {
	width: 64px;
	height: 64px;
	background: #f1f5f9;
	margin: 8px;
}
</style>
```

### Examples Usage

```html
/*vue*/
<template>
	<div id="demo-examples">
		<div class="">
			<nav class="d-flex flex-row">
				<i class="material-icons">menu</i>
				<span class="flex"></span>
				<span>Option</span>
				<span>Option</span>
				<span>Option</span>
			</nav>
		</div>

		<hr>

		<div>
			<div class="card">
				<div class="card-container">
					<p>It means you're hatred, and it also means losing someone, who I've cared for since I first heard his cries echoing through this house. But it might also mean saving your life. And that is more important.</p>

					<p>You want order in Gotham. Batman must take off his mask and turn himself in. Oh, and every day he doesn't, people will die. Starting tonight. I'm a man of my word.</p>

					<p>Batman may have made the front page but Bruce Wayne got pushed to page eight.</p>

					<p>So you came back to die with your city!</p>
				</div>
				<div class="card-actions d-flex flex-row flex-items-end">
					<button>Save</button>
					<button>Cancel</button>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	 export default {
	 }
</script>

<style scoped>
#demo-examples .box-item {
	width: 64px;
	height: 64px;
	background: #f1f5f9;
	margin: 8px;
}

#demo-examples span {
	padding: 8px;
}

#demo-examples .card {
	width:320px;
}
</style>
```