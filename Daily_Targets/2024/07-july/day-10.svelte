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
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffcd;
		--yellow: #edaf38;
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		gap: 140px 20px;
		background-color: var(--yellow);
		grid-template-columns: repeat(6, 50px);
		grid-template-rows: 80px 80px;
		align-items: center;

		& > div {
			height: 80px;
			width: 50px;
			background-color: var(--white);
		}

		& > div:nth-child(7) {
			position: absolute;
			background-color: var(--white);
			height: 100px;
			width: 400px;
		}
	}
</style>
