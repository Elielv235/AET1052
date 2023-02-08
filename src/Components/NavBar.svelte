<script lang="ts">
	// import src from './Logo.png';
</script>

<div class="navbar">
	<div class="navbar-image">
		<img alt="logo" src="/Logo.png" class="Logo" />
	</div>
	<div class="navbar-buttons">
		<a href="#home">בית</a>
		<span>|</span>
		<a href="#about">אודות</a>
		<span>|</span>
		<a href="#research">חקר</a>
		<span>|</span>
		<a href="#Team">חברי הקבוצה</a>
		<span>|</span>
		<a href="#Media">מדיה</a>
	</div>
</div>

<style lang="scss">
	* {
		padding: 0;
		margin: 0;
	}
	.navbar {
		background-color: black;
		color: white;

		position: fixed;

		z-index: 99999;

		left: 0;
		right: 0;
		top: 0;

		padding: 1rem;

		display: flex;
		justify-content: center;

		.navbar-image {
			position: absolute;
			left: 0.6rem;
			top: 0.6rem;
			bottom: 0.6rem;
			img {
				height: 100%;
			}
		}

		.navbar-buttons {
			a {
				text-decoration: none;
				color: white;
				font-size: 1.5rem;

				margin: 0 1rem;

				transition: 0.5s;
				border-radius: 10px;
				// transition-timing-function: cubic-bezier(0.165, 0.84, 0.44, 1);
				&:hover {
					background-color: white;
					color: black;
					padding: 0.55rem;
				}
			}
		}
	}
	@media screen and (max-width: 650px) {
		.navbar {
			.navbar-buttons {
				margin-left: 1rem;

				a {
					margin: 0 5px;
					font-size: 0.8rem;
				}
			}
		}
	}
</style>
