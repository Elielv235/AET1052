<script lang="ts">
	export let num: number;
	const names = [
		'אליאל',
		'אמלי',
		'ליהיא',
		'מאיה',
		'נדב',
		'עופרי',
		'רפאל',
		'רומי',
		'שחר',
		'שי',
		'ולריה',
		'יניב'
	];
</script>

<div class="person">
	<h4 class="unselectable">{names[num - 1]}</h4>
	<img src="/people/{num}.jpeg" class="image" alt={num.toString()} />
</div>

<style lang="scss">
	.person {
		display: grid;

		position: relative;
		z-index: 1;
		flex: 1 0 calc(33% - (1.25rem * 3));

		h4 {
			text-align: center;
			position: absolute;
			top: 0.85rem;
			left: 50%;
			transform: translateX(-50%);
			z-index: 2;

			transition: 0.3s;
		}

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
			h4 {
				font-size: 1.65rem;
			}
		}
	}

	// @media screen and (max-width: 650px) {
	// 	.person:hover {
	// 		.image {
	// 			transform: scale(1);
	// 		}
	// 		h4 {
	// 			font-size: calc(1.275rem + 0.3vw);
	// 		}
	// 	}
	// }

	@media screen and (max-width: 650px) {
		.person {
			flex: 1 0 calc(50% - (1.25rem * 3));
		}
	}
</style>
