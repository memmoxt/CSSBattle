<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--light: #6592cf;
		--dark: #243d83;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--light);
		& > div:nth-child(1) {
			height: 200px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--dark);
			box-shadow:
				-225px 0 var(--dark),
				225px 0 var(--dark);
			opacity: 1;
			z-index: 2;
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 31px;
            width:29px;
			background-color: var(--light);
			/* background-color: red; */
			/* opacity: 0.5; */
			border-radius: 71px/63px;
			box-shadow:
				-0.3px 50px var(--light),
				-226px 0 var(--light),
				-226px 50px var(--light);
			transform: translate(113px, -25px);
			z-index: 3;
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 40px;
			width: 273px;
			background-color: var(--dark);
			opacity: 1;
			z-index: 0;
		}
	}
</style>
