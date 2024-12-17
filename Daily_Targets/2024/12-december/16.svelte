<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--black: #222222;
        background-color:var(--yellow);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			height: 80px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--black);
			box-shadow: 0 0 0 30px var(--yellow);
            z-index:2;
		}
		& > div:nth-child(2) {
            z-index:1;
			position: absolute;
			top: 140px;
			height: 100px;
			width: 100px;
			background-color: var(--black);
			&:before {
				top: 80px;
				left: -75px;
				content: '';
				position: absolute;
				background-color: var(--black);
				height: 30px;
				width: 250px;
			}
		}
	}
</style>

