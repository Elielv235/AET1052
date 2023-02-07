<script lang="ts">
	import { fly } from 'svelte/transition';
	import { expoOut } from 'svelte/easing';
</script>

<div class="welcome">
	<h1 in:fly={{ y: -50, duration: 1500, easing: expoOut, delay: 500 }}>-ברוכים הבאים ל</h1>
	<h1 in:fly={{ x: 150, duration: 1000, easing: expoOut, delay: 750 }}>Agnon</h1>
	<h1 in:fly={{ x: -150, duration: 1000, easing: expoOut, delay: 1000 }}>Energy</h1>
	<h1 in:fly={{ x: 150, duration: 1000, easing: expoOut, delay: 1250 }}>Team</h1>
</div>

<style lang="scss">
	.welcome {
		display: flex;
		height: calc(80vh - 3.5rem);
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
