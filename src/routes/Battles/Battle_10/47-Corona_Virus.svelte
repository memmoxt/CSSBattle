<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div class="circle"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f3ac3c;
		--green: #1a4341;
		--dark: #998235;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--green);
		& > .circle {
			height: 100px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(20px, 20px);
				background-color: var(--dark);
				box-shadow:
					15px 40px 0px -5px var(--dark),
					40px -10px 0px -10px var(--dark);
			}
		}
		& > div:nth-child(1),
		& > div:nth-child(2),
		& > div:nth-child(3) {
			position: absolute;
			height: 180px;
			width: 10px;
			border-radius: 5px;
			transform: translate(0px, -10px);
			background-color: var(--yellow);
		}
		& > div:nth-child(2) {
			transform: translate(8.5px, -5px) rotate(60deg);
		}
		& > div:nth-child(3) {
			transform: translate(8px, 5px) rotate(-60deg);
		}
	}
</style>
