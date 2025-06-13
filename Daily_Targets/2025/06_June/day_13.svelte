<div class="main">
	<div class="circle"></div>
	<div class="square"></div>
	<div class="circle"></div>
	<div class="square"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #d95362;
		--white: #ebf6f0;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > .circle {
			position: absolute;
			height: 130px;
			width: 260px;
			background-color: var(--white);
			transform: translateX(-65px) translateY(65px);
			display: flex;
			justify-content: center;
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translateY(-50%);
				background-color: var(--white);
				box-shadow: 0 0 0 50px var(--red);
			}
		}
		& > .square {
			position: absolute;
			height: 130px;
			transform: translate(-100%, -50%);
			aspect-ratio: 1;
			background-color: var(--red);
		}
		& > div:nth-child(1) {
			transform: translate(65px, -65px) rotate(-180deg);
			background-color: var(--white);
			position: absolute;
		}
		& > div:nth-child(4) {
			transform: translate(130px, 65px) rotate(0deg);
			background-color: var(--red);
		}
	}
</style>
