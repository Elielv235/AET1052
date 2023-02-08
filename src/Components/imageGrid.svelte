<script>
	import People from './Sections/image.svelte';
</script>

<div class="container">
	<h1 style="text-align: center; margin-bottom:20px;">מדיה</h1>
	<div class="row">
		<div class="col-sm">
			{#each Array.from({ length: 10 }, (_, i) => i + 1) as p}
				<People num={p} />
			{/each}
		</div>
		<div class="col-sm">
			{#each Array.from({ length: 10 }, (_, i) => i + 11) as p}
				<People num={p} />
			{/each}
		</div>
		<div class="col-sm">
			{#each Array.from({ length: 6 }, (_, i) => i + 20) as p}
				<People num={p} />
			{/each}
		</div>
	</div>
</div>

<style lang="scss">
	.margin {
	}
</style>
