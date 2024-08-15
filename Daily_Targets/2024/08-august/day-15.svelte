<div class="main">
	<div><div></div></div>
	<div></div>
	<div><div></div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f5bb60;
		--blue: #2f5a76;
		background-color: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1),
		& > div:nth-child(3) {
			position: absolute;
			background-color: var(--yellow);
			height: 110px;
			width: 110px;
			border-radius: 50%;
			transform: translate(2px, -54px) rotate(-45deg);
			clip-path: polygon(0px 0px, 110px 0px, 110px 55px, 0px 55px);
			& > div {
				height: 50px;
				width: 50px;
				background-color: var(--blue);
				border-radius: 50%;
				transform: translate(30px, 30px);
			}
		}
		& > div:nth-child(2) {
			height: 85px;
			width: 30px;
			background-color: var(--yellow);
			position: absolute;
			transform: translate(-0px, 6px) rotate(-40deg);
		}
		& > div:nth-child(3) {
			transform: translate(-8px, 59px) rotate(137deg);
		}
		& > div:nth-child(4) {
			position: absolute;
			height: 30px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 50%;
			transform: translate(32px, -80px);
			box-shadow: -71px 164px 0 var(--yellow);
		}
	}
</style>
