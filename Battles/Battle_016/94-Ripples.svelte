<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #0e2e2c;
		--orange: #f3ac3c;
		--amber: #998235;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--green);
		& > div {
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--orange);
			/* opacity: 0.5; */
			border-radius: 50%;
			box-shadow:
				0 0 0 8px var(--green),
				0 0 0 20px var(--orange),
				0 0 0 30px var(--green),
				0 0 0 40px var(--amber),
				0 0 0 52px var(--green),
				0 0 0 60px var(--orange),
				0 0 0 74px var(--green),
				0 0 0 80px var(--orange);
		}
	}
</style>
