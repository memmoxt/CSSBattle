<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #edaf38;
		--yellow: #ffffcd;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;

		& > div {
			height: 100%;
			width: 50%;
			background: var(--yellow);
			display: flex;
			justify-content: end;
			align-items: center;
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 70px;
				background: var(--orange);
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(-40px, 0px);
				box-shadow: 0px 0px 0px 20px var(--orange);
				background: var(--yellow);
			}
		}
		& > div:nth-child(2) {
			transform: scaleX(-1);
			background: var(--orange);
			&:before {
				background: var(--yellow);
			}
			&:after {
				background: var(--orange);
				box-shadow: 0px 0px 0px 20px var(--yellow);
			}
		}
	}
</style>

