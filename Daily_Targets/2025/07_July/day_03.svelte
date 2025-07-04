<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
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
		box-sizing: content-box;
		--red: #ce636f;
		--pink: #f7bed9;
		--darkred: #b44141;
		background-color: var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		grid-template-columns: repeat(5, 1fr);
		grid-template-rows: repeat(4, 1fr);
		justify-content: center;
		align-items: center;
		overflow: hidden;
		/* opacity: 0.5; */
		& > div {
			height: 80px;
			aspect-ratio: 1;
			background-color: var(--darkred);
		}
		& > div:nth-child(2n + 1) {
			background-color: var(--pink);
		}
		& > div:nth-child(7) {
			border-bottom-left-radius: 50%;
		}
		& > div:nth-child(9) {
			border-bottom-right-radius: 50%;
		}
		& > div:nth-child(6),
		div:nth-child(10) {
			background-color: var(--red);
		}
	}
</style>
