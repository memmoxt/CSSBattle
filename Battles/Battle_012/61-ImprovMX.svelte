<div class="main">
	<div class="top"></div>
	<div class="middle"></div>
	<div class="bottom"></div>
	<div class="water"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5dbcf9;
		--black: #191919;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		background-color: var(--black);
		&:before {
			content: '';
			position: absolute;
			height: 4px;
			aspect-ratio: 1;
			transform: translateY(-21.2px) translateX(-0.2px) rotate(45deg);
			background-color: var(--blue);
			z-index: 10;
		}
		& > .top {
			height: 40px;
			width: 50px;
			border-top: 11px solid var(--blue);
			border-right: 10px solid var(--blue);
			border-left: 10px solid var(--blue);
			border-bottom: 10px solid transparent;
			transform: translateY(-2px);
		}
		& > .middle {
			height: 70px;
			width: 100px;
			transform: translateY(-12px);
			border-top: 11px solid var(--blue);
			border-right: 10px solid var(--blue);
			border-left: 10px solid var(--blue);
			border-bottom: 10px solid transparent;
		}
		& > .bottom {
			height: 45px;
			width: 90px;
			border-top: 10px solid var(--blue);
			border-right: 10px solid var(--blue);
			border-bottom: 10px solid transparent;
			border-left: 10px solid transparent;
			transform: rotate(30deg) translate(7.7px, -42px);
			&:before {
				content: '';
				position: absolute;
				height: 45px;
				width: 70px;
				border-top: 10px solid var(--blue);
				border-left: 10px solid var(--blue);
				border-bottom: 10px solid transparent;
				border-right: 10px solid transparent;
				transform: rotate(-60deg) translate(-37px, -35px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 90px;
				width: 10px;
				border-radius: 33px 39px 0 0;
				background-color: var(--blue);
				/* opacity:0.5; */
				transform: rotate(-30deg) translate(14.6px, -8px);
			}
		}
		& > .water {
			height: 10px;
			width: 200px;
			background-color: var(--blue);
			transform: translate(0, -19px);
			box-shadow:
				0 -10px 0 var(--black),
				0 10px 0 var(--black);
			&:before {
				content: '';
				position: absolute;
				height: 10px;
				width: 110px;
				background-color: var(--blue);
				transform: translate(45px, 20px);
			}
		}
	}
</style>
