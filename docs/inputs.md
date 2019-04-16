# Inputs

# Radio Buttons
```html
<div class="input">
	<input type="radio" id="my-radio" value="My Label text" v-model="textClass">
	<label for="my-radio">My Label text</label>
</div>
```

```html
/*vue*/
<template>
    <div id="demo-text">
        <div class='wrapper'>
					{{selected}}
				</div>
				
				<br>

				<b>Available options</b>
				<div class="d-grid">
					<div class="input">
						<input type="radio" id="batima" value="Batman" v-model="selected">
						<label for="batima">Batman</label>
					</div>
					<div class="input">
						<input type="radio" id="Joker" value="Joker" v-model="selected">
						<label for="Joker">Joker</label>
					</div>
					<div class="input">
						<input type="radio" id="Bane" value="Bane" v-model="selected">
						<label for="Bane">Bane</label>
					</div>
				</div>
    </div>
</template>

<script>
	export default {
		data() {
			return {
				selected: 'Joker'
			}
		}
	}
</script>

<style>
#demo-text .d-grid {
	grid-template-columns: 25% 25% 25% 25%;
}
</style>
```

# Input Search

```html
<div class="input">
	<input type="search">
</div>
```

```html
/*vue*/
<template>
    <div id="demo-text">
        <div class="input">
					<input type="search" placeholder="Type your search here..." />
				</div>
    </div>
</template>

<script>
	export default {
		
	}
</script>
```

# Inputs

```html
<div class="input">
	<input type="text">
</div>

<div class="input">
	<input type="number">
</div>

<div class="input">
	<input type="email">
</div>

<div class="input">
	<input type="phone">
</div>
```

```html
/*vue*/
<template>
    <div id="demo-text">
        <div class="input">
					<input type="text" placeholder="Enter your full name" required>
				</div>

				<div class="input">
					<input type="number" placeholder="Enter your age" min="10" max="24" required>
				</div>

				<div class="input">
					<label class="flex-20">Email</label>
					<input type="email" placeholder="Enter a valid email" required>
				</div>

				<div class="input">
					<label class="flex-20">Phone</label>
					<input type="phone" placeholder="Enter your phone" required>
				</div>

				<div class="input">
					<label for="service">Selecione o Nível de Serviço (SLA)</label>
					<select>
						<option disabled selected>Selecione uma opção</option>
					</select>
				</div>

				<div class="input">
					<label for="service">Selecione um arquivo</label>
					<input type="file">
				</div>

				<div class="input">
					<label for="service">Digite um texto</label>
					<textarea></textarea>
				</div>
    </div>
</template>

<script>
	export default {
		
	}
</script>
```