<div class="main">
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
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--red: #de817e;
		--yellow: #ebe77e;
		background-color: var(--red);
		& > div:nth-child(1) {
			position: absolute;
			clip-path: polygon(0 0, 30px 42px, 60px 0px, 90px 42px, 120px 0px, 120px 100px, 0px 100px);
			height: 100px;
			width: 120px;
			background-color: var(--yellow);
		}
		& > div:nth-child(2) {
			top: 210px;
			position: absolute;
			width: 120px;
			height: 20px;
			background-color: var(--yellow);
		}
	}
</style>
