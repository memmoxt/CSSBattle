<div class="main">
	<div class="brick"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #293462;
		--darkred: #a64942;
		--red: #fe5f55;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--blue);
		& > .brick {
			height: 100px;
			width: 200px;
			background-color: var(--red);
			border-radius: 20px;
			transform: translateY(-10px);
			box-shadow: 0px 20px 0px var(--darkred);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 140px;
				border-radius: 20px;
				transform: translate(30px, 30px);
				background-color: var(--darkred);
			}
		}
	}
</style>
