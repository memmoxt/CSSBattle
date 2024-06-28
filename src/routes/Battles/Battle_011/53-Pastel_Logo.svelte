<div class="main">
	<div>
		<div></div>
	</div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--dark: #19191a;
		--blue: #4f77ff;
		--sky: #9ad5ff;
		--yellow: #f9e492;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--dark);
		& > div:nth-child(1) {
			height: 150px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--blue);
			transform: translate(0, -25px);
			overflow: hidden;
			z-index: 1;
			& > div {
				position: absolute;
				height: 125px;
				width: 75px;
				transform: translate(0px, 75px);
				background-color: var(--sky);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 125px;
			width: 75px;
			transform: translate(-37px, 37px);
			background-color: var(--yellow);
			z-index: 0;
		}
	}
</style>

