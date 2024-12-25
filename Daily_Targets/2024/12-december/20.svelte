<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #3f4869;
		--green: #61a74e;
		background-color: var(--black);
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
			aspect-ratio: 1;
			background-color: var(--black);
			border-radius: 50%;
			box-shadow: 0 0 0 30px var(--green);
			&:before {
				position: absolute;
				content: '';
				height: 80px;
				width: 30px;
				top: 50px;
				left: 185px;
				background-color: var(--green);
			}
		}
	}
</style>

