<div class="main">
	<div class="flower">
		<div class="ball"></div>
		<div class="top-petal"></div>
		<div class="petal"></div>
		<div class="flower-base"></div>
	</div>
	<div class="base"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f9e492;
		--black: #191919;
		--blue: #4f77ff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--black);
		& > .flower {
			height: 110px;
			width: 140px;
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			& > .ball {
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--blue);
				border-radius: 50%;
				transform: translate(0, -50px);
				box-shadow: 0 0 0 10px var(--black);
				z-index: 6;
			}
			& > .top-petal {
				position: absolute;
				height: 30px;
				width: 100px;
				border-radius: 5px 5px 30px 30px;
				background-color: var(--blue);
				box-shadow: 0 0px 0 10px var(--black);
				transform: translate(0, -30px);
				z-index: 5;
			}
			& > .petal {
				position: absolute;
				height: 30px;
				width: 140px;
				transform: translate(0, -10px);
				border-radius: 5px 5px 30px 30px;
				box-shadow: 0 0px 0 10px var(--black);
				background-color: var(--blue);
				z-index: 4;
			}
			& > .flower-base {
				position: absolute;
				height: 100px;
				border-radius: 50%;
				aspect-ratio: 1;
				transform: translate(0, 5px);
				background-color: var(--blue);
				z-index: 3;
			}
		}
		& > .base {
			height: 80px;
			width: 20px;
			background-color: var(--yellow);
			border-radius: 10px;
			transform: translate(0px, 10px);
			z-index: 2;
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(-10px, -30px);
				background-color: var(--yellow);
			}
		}
	}
</style>
