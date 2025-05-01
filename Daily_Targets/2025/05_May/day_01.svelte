<div class="main">
	<div class="">
		<div></div>
	</div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		background-color: var(--blue);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		--blue: #3f4869;
		--yellow: #f4da64;

		& > div:nth-child(1) {
			position: absolute;
			height: 130px;
			width: 260px;
			top: 70px;
			/* background-color: red; */
			display: flex;
			justify-content: center;
			align-items: center;
			overflow: hidden;
			& > div {
				position: absolute;
				height: 160px;
				aspect-ratio: 1;
				background-color: var(--blue);
				border-radius: 50%;
				top: -80px;
				box-shadow: 0 0 0 50px var(--yellow);
				/* opacity:0.5; */
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 50px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			/* opacity:0.5; */
			margin: 20px;
			align-self: flex-start;
			left: 0px;
			box-shadow:
				310px 0 var(--yellow),
				155px 200px var(--yellow);
		}
	}
</style>
