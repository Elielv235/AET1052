<script>
	import Person from './person.svelte';
</script>

<div class="Team">
	<div class="people-grid">
		<h1 style="text-align: center; margin-bottom:20px;">חברי הקבוצה</h1>
		<div class="person-card-container">
			{#each Array.from({ length: 12 }, (_, i) => i + 1) as p}
				<Person num={p} />
			{/each}
		</div>
	</div>
</div>

<style lang="scss">
	.people-grid {
		max-width: 85%;
		margin: 0 auto;
		.person-card-container {
			display: flex;
			flex-wrap: wrap;
			gap: 1.25rem;
			margin: 0 1rem;
		}
	}
</style>
