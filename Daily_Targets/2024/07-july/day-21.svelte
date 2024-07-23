<div class="main">
	<div class="center">
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #0a6190;
		--blue: #328fc1;
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
		background-color: var(--dark);
		& > .center {
			height: 200px;
			width: 200px;
			background: var(--blue);
			display: flex;
			justify-content: center;
			align-items: center;
			clip-path: polygon(
				0px 75px,
				75px 75px,
				75px 0,
				125px 0,
				125px 75px,
				200px 75px,
				200px 125px,
				125px 125px,
				125px 200px,
				75px 200px,
				75px 125px,
				0px 125px
			);
			& > div:nth-child(1),
			div:nth-child(2) {
				position: absolute;
				height: 25px;
				aspect-ratio: 1;
				transform: translate(-50%, -50%);
				background-color: var(--blue);
				box-shadow:
					0 25px 0px var(--dark),
					-25px 0px 0px var(--dark),
					25px 0px 0px var(--dark),
					0px -25px 0px var(--dark);
			}
			& > div:nth-child(2) {
				transform: translate(50%, 50%);
			}
		}
	}
</style>
