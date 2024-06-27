<div class="main">
	<div class="house"></div>
	<div class="door"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #eeb850;
		--light_blue: #6592cf;
		--dark_blue: #243d83;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--light_blue);
		& > .house {
			height: 100px;
			width: 150px;
			border-radius: 0px 0px 10px 10px;
			transform: translateY(50px);
			background-color: var(--dark_blue);
			&:before {
				content: '';
				position: absolute;
				transform: translate(-25px, -200px);
				border-top: 100px solid transparent;
				border-right: 100px solid transparent;
				border-bottom: 100px solid var(--dark_blue);
				border-left: 100px solid transparent;
			}
		}
		& > .door {
			position: absolute;
			height: 10px;
			width: 100px;
			border-radius: 10px;
			background-color: var(--yellow);
			&:after {
				content: '';
				position: absolute;
				height: 50px;
				width: 50px;
				transform: translate(25px, 55px);
				border-radius: 10px 10px 0 0;
				background-color: var(--yellow);
			}
		}
	}
</style>
