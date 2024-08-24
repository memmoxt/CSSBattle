<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #668884;
		--yellow: #fae29e;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			background-color: var(--yellow);
			height: 300px;
			width: 400px;
			clip-path: polygon(0 0, 200px 0px, 200px 300px, 400px 300px, 400px 150px, 0px 150px);
		}
	}
</style>

