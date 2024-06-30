<div class="main">
	<div>
		<div></div>
		<div></div>
	</div>
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5dbcf9;
		--black: #191919;
		--amber: #f2ad43;
		--yellow: #fff58f;
		--orange: #e08027;
		--brown: #824b20;
		background: var(--black);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 25px;
		& > div:nth-child(1) {
			height: 200px;
			width: 125px;
			display: flex;
			align-items: center;
			overflow: hidden;
			& > div:nth-child(1) {
				height: 150px;
				transform-origin: top left;
				transform: translate(25px, 75px) rotate(-45deg);
				aspect-ratio: 1;
				background-color: var(--blue);
			}
			& > div:nth-child(2) {
				position: absolute;
				height: 50px;
				width: 100px;
				border-radius: 10px;
				background-color: var(--blue);
			}
		}
		& > div:nth-child(2) {
			height: 200px;
			width: 100px;
			overflow: hidden;
			display: flex;
			align-items: center;
			& > div:nth-child(1) {
				height: 80px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(-50%, 0);
				background-color: var(--black);
				box-shadow:
					0 0 0 10px var(--blue),
					0 0 0 25px var(--black),
					0 0 0 35px var(--blue),
					0 0 0 50px var(--black),
					0 0 0 60px var(--blue);
			}
		}
	}
</style>
