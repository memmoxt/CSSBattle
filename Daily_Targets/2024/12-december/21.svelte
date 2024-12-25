<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #ea9a52;
		--blue: #435998;
        background-color:var(--orange);
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
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--orange);
			box-shadow: 0 0 0 30px var(--blue);
			transform: rotate(45deg);
			&:before {
				height: 120px;
				width: 30px;
				position: absolute;
				content: '';
				transform: translate(-30px, -70px);
				background-color: var(--blue);
			}
		}
	}
</style>

