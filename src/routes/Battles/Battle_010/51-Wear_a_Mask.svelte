<div class="main">
	<div class="strap"></div>
	<div class="mask"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #293462;
		--white: #fff1c1;
		--red: #fe5f55;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--blue);
		& > .strap {
			position: absolute;
			transform: translate(0, -20px);
			height: 60px;
			width: 270px;
			border-radius: 40px;
			background-color: transparent;
			border: 10px solid var(--white);
		}
		& > .mask {
			height: 100px;
			width: 150px;
			border-radius: 0 0 50px 50px;
			background-color: var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 10px;
				width: 40px;
				border-radius: 5px;
				transform: translate(20px, 20px);
				box-shadow: 0px 20px 0 var(--red);
				background: var(--red);
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--red);
				transform: translate(90px, 40px);
			}
		}
	}
</style>
