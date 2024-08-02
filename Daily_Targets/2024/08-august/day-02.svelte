<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #49c85b;
		--darkgreen: #1f7d3b;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--darkgreen);
			border-radius: 50%;
			transform: translate(150px, 0px);
			box-shadow:
				-50px 0px 0px 10px var(--darkgreen),
				-110px 0px 0px 20px var(--darkgreen),
				-180px 0px 0px 30px var(--darkgreen),
				-260px 0px 0px 40px var(--darkgreen);
		}
	}
</style>
