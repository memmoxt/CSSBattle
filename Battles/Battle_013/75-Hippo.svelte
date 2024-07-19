<div class="main">
	<div class="hypo">
		<div class="ears"></div>
		<div class="nose"></div>
		<div class="head"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--brown: #191919;
		--red: #a64942;
		--red2: #fe5f55;
		--black: #000000;
		background: var(--brown);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > .hypo {
			height: 190px;
			width: 150px;
			position: absolute;
			display: flex;
			justify-content: center;
			& > div {
				position: absolute;
			}
			& > .nose {
				transform: translate(-0px, 90px);
				border-radius: 55px 55px 45px 45px;
				height: 100px;
				width: 150px;
				background-color: var(--red);
				z-index: 2;
				&:before,
				&:after {
					content: '';
					position: absolute;
					height: 20px;
					width: 30px;
					border-radius: 30px/20px;
					background-color: var(--black);
					transform: translate(20px, 25px) rotate(-45deg);
				}
				&:after {
					transform: translate(100px, 25px) rotate(45deg);
				}
			}
			& > .head {
				height: 130px;
				aspect-ratio: 1;
				border-radius: 60px 60px 0px 0px;
				transform: translate(0px, 20px);
				background-color: var(--red2);
				z-index: 1;
				&:before,
				&:after {
					content: '';
					position: absolute;
					height: 10px;
					aspect-ratio: 1;
					border-radius: 50%;
					background-color: var(--black);
					transform: translate(25px, 50px);
				}
				&:after {
					transform: translate(95px, 50px);
				}
			}
			& > .ears,
			& > .ears:before {
				height: 10px;
				width: 20px;
				border-radius: 50px/25px;
				background-color: var(--black);
				box-shadow: 0 0 0 5.12px var(--red2);
				transform: translate(-40px, 25px) rotate(45deg);
				z-index: 0;
			}
			& > .ears:before {
				position: absolute;
				content: '';
				transform: translate(56px, -56px) rotate(-90deg);
			}
		}
	}
</style>
