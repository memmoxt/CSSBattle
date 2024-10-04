<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #e6e9e3;
		--green: #61a74e;
		--darkgreen: #33572b;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap-reverse;
		flex-direction: column;
		& > div:nth-child(1) {
			position: absolute;
			height: 220px;
			box-shadow: 0px 0px 0 10px var(--darkgreen);
			transform: translateY(4px);
			aspect-ratio: 1;
			background-color: var(--green);
			border-radius: 50%;
			&:before {
				content: '';
				position: absolute;
				height: 90px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				top: 65px;
				left: 65px;
				box-shadow: 0 0 0 10px var(--darkgreen);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			top: 35px;
			height: 240px;
			aspect-ratio: 1;
			background-color: var(--white);
			clip-path: polygon(106px 158px, 133px 158px, 174px 250px, 66px 250px);
			z-index: 2;
		}
		& > div:nth-child(3) {
			position: absolute;
			top: 34px;
			height: 240px;
			aspect-ratio: 1;
			background-color: var(--darkgreen);
			border-radius: 50%;
			clip-path: polygon(101px 150px, 138px 150px, 187px 250px, 55px 250px);
			z-index: 1;
		}
		& > div:nth-child(4) {
			position: absolute;
			height: 90px;
			aspect-ratio: 1;
			background-color: var(--white);
			border-radius: 50%;
			top: 109px;
			left: 155px;
			z-index: 4;
		}
	}
</style>
