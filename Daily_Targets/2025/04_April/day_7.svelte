<div class="main">
	<div>
		<div></div>
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
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		--white: #fcebeb;
		--purple: #8e2c88;
		background-color: var(--white);

		& > div {
			height: 72px;
			width: 288px;
			/* background-color: red; */
			display: grid;
			column-gap: 20px;
			grid-template-columns: repeat(7, 1fr);
			grid-template-rows: repeat(3, 1fr);

			& > div {
				background-color: var(--purple);
			}

			& > div:nth-child(1) {
				grid-column: 1/2;
				grid-row: 3;
			}

			& > div:nth-child(2) {
				grid-column: 2/3;
				grid-row: 4/1;
			}

			& > div:nth-child(3) {
				grid-column: 3/4;
				grid-row: 4/3;
			}
			& > div:nth-child(4) {
				grid-column: 4/5;
				grid-row: 4/1;
			}
			& > div:nth-child(5) {
				grid-column: 5/6;
				grid-row: 4/3;
			}
			& > div:nth-child(6) {
				grid-column: 6/7;
				grid-row: 4/1;
			}
			& > div:nth-child(7) {
				grid-column: 7/7;
				grid-row: -1/-2;
			}
		}
	}
</style>

