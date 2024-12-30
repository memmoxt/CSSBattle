<div class="main">
	<div><div></div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--dark: #3f4869;
		--yellow: #efcb5c;
		--amber: #978963;
		background-color: var(--dark);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1),
		& > div:nth-child(1) > div {
			position: absolute;
			overflow: hidden;
			height: 130px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 50%;
		}
		& > div:nth-child(1) > div {
			background-color: var(--dark);
			transform: translate(-101px);
			box-shadow: 0 0 0 30px var(--amber);
		}
		& > div:nth-child(2) {
			position: absolute;
			content: '';
			height: 130px;
			aspect-ratio: 1;
			background-color: var(--dark);
			border-radius: 50%;
			transform: translate(-101px);
            z-index:2;
		}
	}
</style>

