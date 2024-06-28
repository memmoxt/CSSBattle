<div class="main">
	<div class="knuckle">
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
	<div class="palm"></div>
	<div class="wrist"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		--yellow: #f9e492;
		--black: #191919;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--yellow);
		& > .knuckle {
			height: 65px;
			width: 100px;
			display: grid;
			grid-template-columns: repeat(4, auto);
			justify-items: end;
			align-items: end;
			& > div,
			& > div:nth-child(2):after {
				height: 45px;
				width: 20px;
				border-radius: 20px;
				margin-bottom: 5px;
				background-color: var(--black);
			}
			& > div:nth-child(2) {
				height: 55px;
				&:after {
					content: '';
					position: absolute;
					background-color: var(--black);
					height: 64px;
					width: 20px;
					border: 5px solid var(--yellow);
					transform: translate(-28px, 28px) rotate(60deg);
				}
			}

			& > div:nth-child(4) {
				height: 35px;
			}
		}
		& > .palm {
			height: 40px;
			width: 100px;
			background-color: var(--black);
			border-radius: 0 0 10px 10px;
		}
		& > .wrist {
			height: 50px;
			width: 50px;
			background-color: var(--black);
			border-radius: 0 0 10px 10px;
			transform: translate(0, -5px);
		}
	}
</style>
