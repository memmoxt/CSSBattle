<!-- https://cssbattle.dev/play/104 -->
<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #000000;
		--dark: #37385a;
		--light: #9897ae;
		--white: #c0c3db;
		background-color: var(--black);
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
			width: 200px;
			border-radius: 10px/10px;
			background-color: var(--light);
			z-index: 2;
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				width: 52px;
				transform: skewX(-15deg);
				background-color: var(--white);
				translate: 75px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 10px;
				aspect-ratio: 1;
				background-color: var(--black);
				translate: 15px 15px;
				border-radius: 50%;
				box-shadow:
					0 20px var(--black),
					0 40px var(--black),
					160px 0px var(--black),
					160px 20px var(--black),
					160px 40px var(--black);
			}
		}
		& > div:nth-child(2) {
			z-index: 1;
			position: absolute;
			background-color: var(--dark);
			height: 120px;
			width: 240px;
			border-radius: 20px/20px;
		}
		& > div:nth-child(3) {
			position: absolute;
			z-index: 3;
			height: 50px;
			width: 10px;
			border-radius: 20px;
			translate: -30px;
			box-shadow:
				20px 0px var(--black),
				40px 0px var(--black),
				60px 0px var(--black);
			background-color: var(--black);
		}
	}
</style>
