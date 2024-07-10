<div class="main">
	<div class="skew"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #328fc1;
		--dark: #0a6190;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		background-color: var(--dark);
		& > .skew {
			height: 100px;
			width: 200px;
			background-color: var(--blue);
			transform: skewX(-26.5deg);
		}
		& > .skew:before {
			content: '';
			position: absolute;
			height: 100px;
			width: 200px;
			transform: translate(300px, 0px) skewX(45deg);
			background-color: var(--blue);
		}

		& > .skew:after {
			content: '';
			position: absolute;
			height: 100px;
			width: 200px;
			transform: translate(-300px, 0px) skewX(45deg);
			background-color: var(--blue);
		}
	}
</style>
