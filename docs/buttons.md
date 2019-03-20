# Buttons
We have predefined button styles, each serving its own semantic purpose.

```html
<button class="btn btn-icon">Button</button>
<a href="#" class="btn btn-icon">Button</a>
```

```html
/*vue*/

<template>
	<div id="demo-btns" class="d-grid">
		<button class="btn">Default</button>
		<button class="btn btn-primary">.btn-primary</button>
		<button class="btn btn-secondary">.btn-secondary</button>
		<button class="btn btn-tertiary">.btn-tertiary</button>
		<button class="btn btn-danger">.btn-danger</button>
		<button class="btn btn-warning">.btn-warning</button>
	</div>
</template>

<script>
export default {}
</script>

<style>
#demo-btns {
	grid-template-columns: auto auto auto auto;
}
</style>
```

## Button Text Only

Add class ```.text``` to keep text color only.
```html
<button class="btn btn-icon text">Button</button>
```

```html
/*vue*/

<template>
	<div id="demo-btns" class="d-grid">
		<button class="btn text">Default</button>
		<button class="btn btn-primary text">.btn-primary</button>
		<button class="btn btn-secondary text">.btn-secondary</button>
		<button class="btn btn-tertiary text">.btn-tertiary</button>
		<button class="btn btn-danger text">.btn-danger</button>
		<button class="btn btn-warning text">.btn-warning</button>
	</div>
</template>

<script>
export default {}
</script>

<style>
#demo-btns {
	grid-template-columns: auto auto auto auto;
}
</style>
```

## Icon Button
Add class ```.btn-icon``` to allow icon usage

```html
<button class="btn btn-icon">
	<i class="your-icon-collection">my_icon</i>
</button>
```

```html
/*vue*/

<template>
	<div id="demo-btns" class="d-grid">
		<div class="text-center"><button class="btn btn-icon"><i class="material-icons">menu</i></button></div>
		<div class="text-center"><button class="btn btn-primary btn-icon"><i class="material-icons">done</i></button></div>
		<div class="text-center"><button class="btn btn-secondary btn-icon"><i class="material-icons">language</i></button></div>
		<div class="text-center"><button class="btn btn-tertiary btn-icon"><i class="material-icons">https</i></button></div>
		<div class="text-center"><button class="btn btn-danger btn-icon"><i class="material-icons">favorite</i></button></div>
		<div class="text-center"><button class="btn btn-warning btn-icon"><i class="material-icons">warning</i></button></div>
	</div>
</template>

<script>
export default {}
</script>

<style>
#demo-btns {
	grid-template-columns: auto auto auto auto;
}
</style>
```

## Disabled Button
Add class ```.btn-disabled``` or add attribute ```disabled``` to allow icon usage

```html
<button disabled class="btn">Button</button>
<button class="btn btn-disabled">Button</button>
```

```html
/*vue*/

<template>
	<div id="demo-btns" class="d-grid">
		<div class="text-center"><button disabled class="btn btn-icon"><i class="material-icons">menu</i></button></div>
		<div class="text-center"><button disabled class="btn btn-primary btn-icon"><i class="material-icons">done</i></button></div>
		<div class="text-center"><button disabled class="btn btn-secondary btn-icon"><i class="material-icons">language</i></button></div>
		<button disabled class="btn btn-tertiary text">.btn-tertiary</button>
		<button disabled class="btn btn-danger text">.btn-danger</button>
		<button disabled class="btn btn-warning text">.btn-warning</button>
		<button disabled class="btn btn-tertiary">.btn-tertiary</button>
		<button disabled class="btn btn-danger">.btn-danger</button>
		<button disabled class="btn btn-warning">.btn-warning</button>
	</div>
</template>

<script>
export default {}
</script>

<style>
#demo-btns {
	grid-template-columns: auto auto auto auto;
}
</style>
```