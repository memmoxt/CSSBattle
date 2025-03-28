<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #00b0c8;
		--white: #ffffff;
		--dark: #1a353c;
        background-color:var(--blue);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > div {
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--white);
			box-shadow: 0 0 0 20px var(--dark);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				width: 300px;
				background-color: white;
				transform: translate(-100px, 40px);
			}
		}
	}
</style>

