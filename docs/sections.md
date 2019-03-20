# Sections

Sessions are used to separate segments from the screen, use to give a context in the flow of your page.

## Definition
```html
<section aria-label="Section Name">
	<div class="section-container"></div>
</section>
```

## Full Example

```html
/*vue*/

<template>
	<div id="demo-full-example" class="d-flex d-column">
		<nav class="side-nav flex-33">
			<ul>
				<li>
					<a @click="setSection('settings')" :class="{'active': section == 'settings'}">Settings</a>
				</li>
				<li>
					<a @click="setSection('security')" :class="{'active': section == 'security'}">Security</a>
				</li>
				<li>
					<a @click="setSection('other-settings')" :class="{'active': section == 'other-settings'}">Other Settings</a>
				</li>
			<ul>
		</nav>
		<main class="flex">
			<section v-if="section == 'settings'" aria-label="Settings">
				<div class="section-container">
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-168"></div>
					<div class="placeholder rect s-240"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-48"></div>
					<div class="placeholder rect s-120"></div>
				</div>
			</section>

			<section v-if="section == 'settings'" aria-label="Settings - Account">
				<div class="section-container">
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-168"></div>
					<div class="placeholder rect s-48"></div>
					<div class="placeholder rect s-120"></div>
				</div>
			</section>

			<section v-if="section == 'security'" aria-label="Security">
				<div class="section-container">
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-168"></div>
					<div class="placeholder rect s-240"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-48"></div>
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-240"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-48"></div>
					<div class="placeholder rect s-120"></div>
				</div>
			</section>

			<section v-if="section == 'other-settings'" aria-label="Other Settings">
				<div class="section-container">
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-168"></div>
					<div class="placeholder rect s-240"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-48"></div>
					<div class="placeholder rect s-120"></div>
					<div class="placeholder rect s-240"></div>
					<div class="placeholder rect s-216"></div>
					<div class="placeholder rect s-216"></div>
				</div>
			</section>
		</main>
	</div>
</template>

<script> 
export default {
	data() {
		return {
			section: 'settings'
		}
	},
	methods: {
		setSection(_section) {
			this.section = _section;
		}
	}
}; 
</script>

<style>
	#demo-full-example {
		width: 100%;
		height: 480px;
		padding: 8px;
	}

	#demo-full-example 	.side-nav {
		background: #fff;
		margin:8px 8px 0;
	}

	#demo-full-example main {
		overflow: auto;
	}
</style>

```