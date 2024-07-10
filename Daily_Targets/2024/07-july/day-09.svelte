<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #4f77ff;
		--white: #eff8fe;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: start;
		align-items: start;
		overflow: hidden;
		position: absolute;
		& > div {
			position: absolute;
			border-top: 0px solid var(--blue);
			border-right: 0px solid var(--blue);
			border-bottom: 50px solid var(--blue);
			border-left: 50px solid var(--blue);
			background-color: var(--white);
			height: 250px;
			width: 400px;
		}
		& > div:nth-child(2) {
			transform: translate(100px, -100px);
		}
		& > div:nth-child(3) {
			transform: translate(200px, -200px);
		}
	}
</style>
