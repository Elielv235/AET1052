<script lang="ts">
	export let num: number;
</script>

<div id="people">
	<img src="/{num}.jpeg" class="image" alt={num.toString()} />
</div>

<style lang="scss">
	#people {
		max-width: 1024px;
		display: grid;

		.image {
			width: 100%;
		}
	}
</style>
