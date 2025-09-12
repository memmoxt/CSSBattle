<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #4a9a86;
		--yellow: #fae29e;
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
			height: 100px;
			width: 30px;
			background-color: var(--green);
			translate: -65px;
			box-shadow:
				-30px 30px var(--green),
				-60px 60px var(--green),
				130px 0px var(--green),
				160px -30px var(--green),
				190px -60px var(--green);
		}
	}
</style>
