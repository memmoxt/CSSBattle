<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #328fc1;
		--darkblue: #0a6190;
		background: var(--darkblue);
	}

	.main {
		height: 100vh;
		width: 100vw;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			height: 119px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(-20px, -170px);
				background-color: var(--blue);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--darkblue);
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 160px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--blue);
			transform: translate(0, 150px);
		}
	}
</style>
