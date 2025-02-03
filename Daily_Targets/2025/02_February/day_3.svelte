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
		--purple: #9076d8;
		--yellow: #f5e3b5;
		background-color: var(--purple);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > div {
			position: absolute;
			top: 60px;
			height: 240px;
			width: 80px;
			background-color: var(--yellow);
			& > div {
				position: absolute;
				top: 0px;
				border-top: 0px solid var(--yellow);
				border-right: 40px solid var(--yellow);
				border-bottom: 40px solid var(--purple);
				border-left: 40px solid var(--yellow);
			}
			& > div:nth-child(2) {
				top: 40px;
			}
			& > div:nth-child(3) {
				top: 160px;
			}
			& > div:nth-child(4) {
				top: 200px;
			}
		}
	}
</style>

