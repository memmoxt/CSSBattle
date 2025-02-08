<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #edecc1;
		--red: #cc5252;
		background-color: var(--yellow);
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
			height: 150px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--yellow);
			box-shadow: 0 0 0 50px var(--red);
			transform: rotate(-30deg);

			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 200px;
				background-color: var(--red);
				top: 50px;
				left: -22px;
			}
		}
	}
</style>
