<script lang="ts">
	export let num: number;
</script>

<div class="person">
	<img src="/{num}.jpeg" class="image" alt={num.toString()} />
</div>

<style lang="scss">
	@media screen and (max-width: 1024px) {
		.person:hover .image {
			transform: scale(1);
		}
	}

	.person {
		display: grid;

		.image {
			margin-top: 5px;
			margin-bottom: 5px;
			border-radius: 10px;
			width: 100%;

			transition: 0.3s;
		}

		&:hover {
			.image {
				transform: scale(1.03);
			}
		}
	}
</style>
