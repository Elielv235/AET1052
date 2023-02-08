<script lang="ts">
	export let num: number;
</script>

<div id="people">
	<img src="/{num}.jpeg" class="image" alt={num.toString()} />
</div>

<style lang="scss">
	#people {
		display: grid;

		.image {
			margin-top: 5px;
			margin-bottom: 5px;
			border-radius: 10px;
			width: 100%;
		}
	}
</style>
