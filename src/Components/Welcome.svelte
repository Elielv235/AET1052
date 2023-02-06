<script lang="ts">
	import { fly } from 'svelte/transition';
	import { expoOut } from 'svelte/easing';
</script>

<div id="welcome">
	<h1 in:fly={{ y: -25, duration: 500, easing: expoOut, delay: 250 }}>Welcome to</h1>
	<h1 in:fly={{ x: 150, duration: 750, easing: expoOut, delay: 750 }}>Agnon</h1>
	<h1 in:fly={{ x: -150, duration: 750, easing: expoOut, delay: 1000 }}>Energy</h1>
	<h1 in:fly={{ x: 150, duration: 750, easing: expoOut, delay: 1250 }}>Team</h1>
</div>

<style lang="scss">
	#welcome {
		display: flex;
		height: 100vh;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		:first-child {
			margin: 1rem 0;
		}
		h1 {
			font-size: 3rem;
		}
	}
</style>