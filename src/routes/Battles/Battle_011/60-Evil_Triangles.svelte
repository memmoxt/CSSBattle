<div class="main">
	<div class="guide">
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f9e492;
		--black: #191919;
		--blue: #4f77ff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--black);
		& > .guide {
			height: 150px;
			width: 200px;
			/* border:1px solid red; */
			overflow: hidden;
			display: flex;
			& > div {
				height: 100px;
				aspect-ratio: 1;
				/* opacity:0.5; */
				transform-origin: top left;
			}
			& > div:nth-child(1) {
				background-color: var(--blue);
				transform: rotate(45deg) translate(-29px, -101px);
				box-shadow: 70px -70px 0 var(--blue);
				z-index: 2;
			}
			& > div:nth-child(2) {
				background-color: var(--black);
				transform: rotate(45deg) translate(-65px, 5px);
				box-shadow: 71px -69px 0 var(--black);
				z-index: 1;
			}
			& > div:nth-child(3) {
				background-color: var(--blue);
				transform: rotate(45deg) translate(-100px, 112px);
				box-shadow:
					70px -70px 0 var(--blue),
					59px -78px 0 var(--blue),
					-15px -5px 0 var(--blue);
				z-index: 0;
			}
		}
	}
</style>
