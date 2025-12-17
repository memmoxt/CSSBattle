<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #45b45b;
		--dark: #194247;
		--red: #e3473c;
		--yellow: #fabc0d;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			height: 180px;
			width: 260px;
			background-color: var(--dark);
			border-radius: 20px;
			&:before {
				height: 20px;
				width: 80px;
				background-color: var(--yellow);
				content: '';
				position: absolute;
				translate: 170px 50px;
				box-shadow:
					0px 30px var(--red),
					-40px 30px var(--red),
					0 60px var(--green),
					-80px 60px var(--green);
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--green);
				border-radius: 50%;
				translate: 10px 10px;
				box-shadow:
					30px 0px var(--yellow),
					60px 0px var(--red);
			}
		}
	}
</style>
