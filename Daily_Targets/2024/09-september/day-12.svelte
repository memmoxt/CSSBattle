<div class="main">
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
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		grid-template-rows: 1fr 1fr;
		grid-template-columns: 1fr 1fr;
		row-gap: 200px;
		column-gap: 10px;
		justify-content: center;
		align-items: center;
		--pink: #f8d2d1;
		--purple: #9076d8;
        background-color:var(--pink);
		& > div {
			height: 50px;
			width: 100px;
			background-color: var(--purple);
			border-bottom-left-radius: 20px;
			border-bottom-right-radius: 20px;
		}
		& > div:nth-child(1) {
			align-self: start;
			justify-self: end;
		}
		& > div:nth-child(2) {
			align-self: start;
		}
		& > div:nth-child(3) {
			transform: scaleY(-1);
			justify-self: end;
		}
		& > div:nth-child(4) {
			transform: scaleY(-1);
		}
	}
</style>

