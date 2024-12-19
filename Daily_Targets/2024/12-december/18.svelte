<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fae29e;
		--orange: #ea9a52;
		background-color: var(--yellow);
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
			position: absolute;
			left: 100px;
			border-top: 70px solid var(--yellow);
			border-right: 85px solid var(--orange);
			border-bottom: 70px solid var(--yellow);
			border-left: 0px solid var(--yellow);
		}
		& > div:nth-child(2) {
			left: 215px;
			transform: scale(-1);
		}
	}
</style>

