<div class="main">
	<div class="base"></div>
	<div class="keys">
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
	<div class="black-keys">
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #998235;
		--black: #191919;
		--white: #ffffff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--yellow);
	}

	.base {
		position: absolute;
		height: 100px;
		width: 180px;
		border-radius: 10px;
		background-color: var(--black);
		/* opacity: 0.5; */
	}

	.keys {
		position: absolute;
		height: 80px;
		width: 180px;
		display: grid;
		/* background-color:black; */
		transform: translate(0px, 10px);
		grid-template-columns: repeat(7, 1fr);
		grid-template-rows: 1fr;
		box-sizing: border-box;
		padding: 5px;
		gap: 5px;

		& > div {
			position: relative;
			background-color: var(--white);
			border-radius: 5px;
			/* opacity: 0.5; */
		}
	}

	.black-keys {
		position: absolute;
		/* background-color: var(--black); */
		/* opacity: 0.5; */
		height: 35px;
		transform: translate(0, -8px);
		width: 140px;
		padding: 0;
		gap: 10px;
		display: grid;
		grid-template-columns: repeat(6, 15px);
		grid-template-rows: 1fr;

		& > div {
			position: relative;
			height: 35px;
			width: 15px;
			background-color: var(--black);
		}
		& > div:nth-child(3) {
			background-color: transparent;
		}
	}
</style>
