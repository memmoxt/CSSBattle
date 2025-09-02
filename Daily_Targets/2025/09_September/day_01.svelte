<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f4da64;
		--red: #e25c57;
		background-color: var(--red);
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
			height: 30px;
			width: 200px;
			background-color: var(--yellow);
			translate: -100px 35px;
			box-shadow:
				0 50px var(--yellow),
				0 100px var(--yellow),
				200px -70px var(--yellow),
				200px -120px var(--yellow),
				200px -170px var(--yellow);
		}
	}
</style>
