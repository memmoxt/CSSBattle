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
		box-sizing: content-box;
		--yellow: #f9e492;
		--black: #191919;
		--blue: #4f77ff;
		background-color: var(--black);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;

		& > div:nth-child(1) {
			position: absolute;
			height: 200px;
			aspect-ratio: 1;
			/* opacity: 0.5; */
			overflow: hidden;
			border-radius: 50%;
			z-index: 1;

			& > div {
				transform: translate(-52px, -60px);
				position: absolute;
				border-top: 170px solid var(--yellow);
				border-right: 152px solid var(--yellow);
				border-left: 152px solid var(--yellow);
				border-bottom: 152px solid var(--black);
			}
		}

		& > div:nth-child(2) {
			z-index: 0;
			overflow: visible;
			background-color: red;
			position: absolute;
			border-top: 170px solid var(--black);
			border-right: 152px solid var(--black);
			border-left: 152px solid var(--black);
			border-bottom: 152px solid var(--blue);
			/* opacity:0.5; */
		}
	}
</style>
