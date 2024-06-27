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
		--orange: #ea7457;
		--red: #b53733;
	}

	.main {
		height: 300px;
		width: 400px;
		display: grid;
		grid-template-columns: 1fr 200px 1fr;
		grid-template-rows: repeat(3, 1fr);
		background: var(--orange);

		& > div {
			height: 100px;
			width: 100px;
			background-color: var(--red);
		}
		& > div:nth-child(1) {
			grid-column: 2/3;
			justify-self: center;
		}
		& > div:nth-child(2) {
			grid-column: 1;
			grid-row: 2;
		}
		& > div:nth-child(3) {
			grid-column: 3;
			grid-row: 2;
		}
		& > div:nth-child(4) {
			grid-column: 2;
			grid-row: 3;
			justify-self: center;
		}
		& > div:nth-child(5),
		& > div:nth-child(5):before {
			position: absolute;
			height: 300px;
			width: 20px;
			background-color: var(--red);
			justify-self: center;
		}
		& > div:nth-child(5):before {
			content: '';
			position: absolute;
			transform: rotate(90deg);
		}
	}
</style>
