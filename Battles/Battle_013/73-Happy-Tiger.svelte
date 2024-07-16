<div class="main">
	<div class="ears"></div>
	<div class="head">
		<div class="hair"></div>
		<div class="eyes"></div>
		<div class="mouth"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f3ac3c;
		--beige: #998235;
		--green: #1a4341;
		--white: #ffffff;
		background: var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
		}
		& > .head {
			height: 150px;
			width: 150px;
			border-radius: 75px 75px 60px 60px;
			background-color: var(--beige);
			display: flex;
			justify-content: center;
			align-items: center;
			overflow: hidden;
			& > .hair {
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--green);
				transform: rotate(45deg) translate(-60px, -60px);
			}
			& > .eyes {
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(40px, -5px);
				background-color: var(--green);
				box-shadow: -80px 0 0 0px var(--green);
			}
			& > .mouth {
				z-index: 3;
				height: 40px;
				width: 100px;
				transform: translate(0, 40px);
				border-radius: 20px 20px 50px 50px;
				background-color: var(--white);
				&:before {
					content: '';
					position: absolute;
					height: 20px;
					aspect-ratio: 1;
					border-radius: 50%;
					transform: translate(25px, 0px);
					background-color: var(--white);
					box-shadow:
						0 0 0 10px var(--green),
						30px 0 0 0px var(--white),
						30px 0 0 10px var(--green);
					clip-path: polygon(-15px 10px, 60px 10px, 60px 30px, -15px 30px);
				}
				&:after {
					content: '';
					position: absolute;
					height: 30px;
					width: 10px;
					background-color: var(--green);
					transform: translate(45px, -10px);
				}
			}
		}
		& > .ears,
		& > .ears:before {
			z-index: 0;
			height: 40px;
			aspect-ratio: 1;
			border-radius: 50%;
			transform: translate(55px, -55px);
			background-color: var(--green);
			box-shadow: 0 0 0 10px var(--beige);
		}
		& > .ears:before {
			position: absolute;
			content: '';
			transform: scaleX(-1) translate(110px, 0px);
		}
	}
</style>
