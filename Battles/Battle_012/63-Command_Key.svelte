<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
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
		display: grid;
		justify-content: center;
		align-content: center;
		justify-items: center;
		align-items: center;
		grid-template-columns: repeat(3, 50px);
		grid-template-rows: repeat(3, 50px);
		gap: 10px;
		transform: translate(0px, -1px);

		& > div {
			height: 70px;
			aspect-ratio: 1;
			border: 10px solid var(--blue);
			background-color: var(--black);
			border-radius: 50%;
			/* opacity:0.5; */
		}
		& > div:nth-child(1) {
			grid-column: 1/2;
			border-bottom-right-radius: 0%;
			transform: translate(1px, 0px);
		}

		& > div:nth-child(2) {
			grid-column: 3/-1;
			border-bottom-left-radius: 0%;
			transform: translate(1px, 0px);
		}
		& > div:nth-child(3) {
			grid-row: 2;
			grid-column: 2;
			border-radius: 0;
			transform: translate(1px, 0px);
		}
		& > div:nth-child(4) {
			grid-row: 3;
			grid-column: 1;
			border-top-right-radius: 0;
			transform: translate(1px, 0px);
		}
		& > div:nth-child(5) {
			grid-row: 3;
			grid-column: -2;
			border-top-left-radius: 0;
			transform: translate(1px, 0px);
		}
	}
</style>
