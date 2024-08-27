<div class="main">
	<div>
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
		box-sizing: border-box;
		--orange: #ea9a52;
		--blue: #555fd9;
        background-color:var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 200px;
			width: 300px;
			display: grid;
			grid-template-columns: 1fr 1.5fr 1fr 1.5fr 1fr;
			grid-template-rows: repeat(4, 1fr);
			& > div {
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--blue);
			}
			& > div:nth-child(2) {
				grid-column-start: 3;
			}
			& > div:nth-child(3) {
				grid-column-start: -2;
			}
			& > div:nth-child(5) {
				grid-column-start: 3;
			}
			& > div:nth-child(6) {
				grid-column-start: 5;
			}
			& > div:nth-child(4),
			div:nth-child(5),
			div:nth-child(6) {
				grid-row-start: -2;
			}
		}
	}
</style>

