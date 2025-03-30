<div class="main">
	<div>
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
		--red: #e25c57;
		--yellow: #eddf5a;
		background-color: var(--red);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;

		& > div {
			height: 100px;
			width: 130px;
			display: grid;
			column-gap: 10px;
			grid-template-columns: repeat(4, 25px);
			grid-template-rows: repeat(4, 25px);
			& > div {
				background-color: var(--yellow);
			}
			& > div:nth-child(1) {
				grid-column: 1/2;
				grid-row: 4/5;
			}
			& > div:nth-child(2) {
				grid-column: 2/3;
				grid-row: 3/5;
			}
			& > div:nth-child(3) {
				grid-column: 3/4;
				grid-row: 2/5;
			}
			& > div:nth-child(4) {
				grid-column: -1/-2;
				grid-row: 1/5;
			}
		}
	}
</style>

