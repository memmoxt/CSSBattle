<div class="main">
	<div class="box">
		<div class="top">
			<div class="top-border"></div>
			<div class="ball-top"></div>
		</div>
		<div class="center">
			<div class="center-box"></div>
			<div class="ball-center"></div>
			<div class="ball-center"></div>
		</div>
		<div class="bottom">
			<div class="bottom-border"></div>
			<div class="ball-bottom"></div>
		</div>
	</div>
</div>
<style>
	* {
		background: #09042a;
		margin: 0;
	}

	.main {
		display: flex;
		height: 100vh;
		justify-content: center;
		align-items: center;

		.box {
			width: 50vw;
			height: 60vh;
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: space-between;

			.top {
				height: 80px;
				width: 20vw;
				z-index: 10;
				margin-bottom: -60px;
				background-color: transparent;

				.ball-top {
					height: 60px;
					aspect-ratio: 1;
					background-color: #f5bb9c;
					border-radius: 50%;
					transform: translate(10px, 7px);
					border: 0px solid #09042a;
				}
			}

			.top-border {
				position: absolute;
				height: 85px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(-2.5px, -8px);
				background-color: #09042a;
			}

			.center {
				height: 80px;
				width: 200px;
				display: flex;
				justify-content: space-between;
				align-items: center;

				.ball-center {
					height: 60px;
					aspect-ratio: 1;
					background-color: #09042a;
					border-radius: 50%;
					border: 10.5px solid #e78481;
					z-index: 20;
				}

				.center-box {
					height: 50px;
					width: 120px;
					background-color: #e78481;
					position: absolute;
					transform: translate(40px, 0px);
				}
			}

			.bottom {
				height: 80px;
				width: 20vw;
				z-index: 10;
				margin-top: -60px;
				background-color: transparent;

				.ball-bottom {
					height: 60px;
					aspect-ratio: 1;
					background-color: #f5bb9c;
					border-radius: 50%;
					transform: translate(10px, 13px);
				}

				.bottom-border {
					position: absolute;
					height: 85px;
					aspect-ratio: 1;
					border-radius: 50%;
					transform: translate(-2.5px, 2.5px);
					background-color: #09042a;
				}
			}
		}
	}
</style>
