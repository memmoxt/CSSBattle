<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #51a499;
		--yellow: #eac049;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color: var(--yellow);
        overflow: hidden;
		& > div {
			position: absolute;
			left: 0px;
			height: 180px;
			width: 230px;
			background-color: var(--green);
			box-shadow:
				230px -180px var(--green),
				230px 180px var(--green);
		}
	}
</style>

