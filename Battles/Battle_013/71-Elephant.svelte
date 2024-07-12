<div class="main">
	<div class="ears"></div>
	<div class="ears"></div>
	<div class="face"></div>
	<div class="eye"></div>
	<div class="eye"></div>
	<div class="tusk"></div>
	<div class="trunk"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		--yellow: #998235;
		--green: #1a4341;
		--dark: #0b2429;
		--white: #ffffff;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--yellow);
		& > .ears {
			transform: translate(-73px, 0);
			height: 180px;
			width: 80px;
			clip-path: ellipse(40px 90px at 54% 50%);
			background-color: var(--green);
			z-index: 0;
			&:before {
				transform: translate(16px, 0);
				position: absolute;
				content: '';
				height: 180px;
				width: 80px;
				clip-path: ellipse(40px 90px at 54% 50%);
				background-color: var(--dark);
				z-index: 1;
			}
		}
		& > .ears:nth-child(2) {
			transform: scaleX(-1) translate(-73px, 0);
		}
		& > .face {
			position: absolute;
			border-radius: 50%;
			height: 180px;
			aspect-ratio: 1;
			background-color: var(--green);
		}
		& > .eye {
			position: absolute;
			transform: translate(-30px, 0px);
			height: 40px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--yellow);
			clip-path: polygon(0% 100%, 100% 100%, 100% 50%, 0% 50%);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(50%, 50%);
				background-color: var(--dark);
			}
		}
		& > .eye:nth-child(4) {
			transform: translate(30px, 0) scaleX(-1);
		}
		& > .tusk {
			position: absolute;
			height: 60px;
			width: 120px;
			transform: translate(0px, 70px);
			overflow: hidden;

			&:before {
				content: '';
				position: absolute;
				border-radius: 50%;
				height: 80px;
				aspect-ratio: 1;
				border: 20px solid var(--white);
			}
		}
		& > .trunk {
			position: absolute;
			height: 120px;
			width: 40px;
			transform: translate(0, 90px);
			border-radius: 50px 50px 0 0;
			background-color: var(--dark);
		}
	}
</style>
