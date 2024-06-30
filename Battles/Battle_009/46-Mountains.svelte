<div class="main">
	<div class="circle">
		<div class="square"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #293462;
		--red: #fe5f55;
		--yellow: #fff1c1;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--blue);
		& > .circle {
			height: 200px;
			aspect-ratio: 1;
			border-radius: 50%;
			overflow: hidden;
			background-color: var(--yellow);
			& > .square {
				height: 130px;
				aspect-ratio: 1;
				transform: translate(50px, 150px) rotate(-45deg);
				transform-origin: top left;
				background-color: var(--red);
				box-shadow: -130px -30px 0px var(--red);
			}
		}
	}
</style>
