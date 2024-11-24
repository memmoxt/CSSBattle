<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #328fc1;
		--yellow: #eeb850;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 20px;
			width: 100px;
			background-color: var(--yellow);
			box-shadow:
				-124px 22px 0 var(--yellow),
				-124px -22px 0 var(--yellow),
				124px 22px var(--yellow),
				124px -22px var(--yellow);
		}
	}
</style>

