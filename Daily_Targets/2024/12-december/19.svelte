<div class="main">
	<div>
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
		box-sizing: border-box;
		--black: #35312f;
		--pink: #cf81af;
		background-color: var(--black);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			gap: 20px;
			height: 160px;
			aspect-ratio: 1;
			display: grid;
			grid-template-rows: repeat(3, 1fr);
			grid-template-columns: repeat(3, 1fr);
			& > div {
				height: 100%;
				aspect-ratio: 1;
				background-color: var(--pink);
			}
			& > div:nth-child(1) {
				grid-row: 3/4;
				grid-column: 2/3;
			}
			& > div:nth-child(2) {
				grid-row: 2/3;
				grid-column: 3/4;
			}
			& > div:nth-child(3) {
				grid-row: 2/3;
				grid-column: 2/3;
			}
			& > div:nth-child(4) {
				grid-row: 2/3;
				grid-column: 1/2;
			}
			& > div:nth-child(5) {
				grid-row: 1/2;
				grid-column: 2/3;
			}
		}
	}
</style>
