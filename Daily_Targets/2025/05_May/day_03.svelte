<div class="main">
	<div class=""></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f4da64;
		--green: #5c8d8f;
        background-color: var(--green);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 160px;
			aspect-ratio: 1;
			background-color: var(--green);
			top: -80px;
			border-radius: 50%;
			box-shadow:
				0 300px var(--green),
				0 0 0 50px var(--yellow),
				-200px 150px 0 50px var(--yellow),
				0px 300px 0 50px var(--yellow),
				200px 150px 0 50px var(--yellow);
		}
	}
</style>

