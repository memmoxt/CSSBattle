<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--green: #61a74e;
		--white: #ffffff;
		background-color: var(--green);
		& > div {
			position: absolute;
			left: 50px;
			height: 200px;
			width: 140px;
			background-color: var(--green);
			box-shadow: 0 0 0 20px var(--white);
			&:before {
				position: absolute;
				content: '';
				right: -30px;
				top: 80px;
				height: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--green);
				box-shadow: 0 0 0 20px var(--white);
			}
			&:after {
				position: absolute;
				content: '';
				top: 70px;
				height: 60px;
				width: 20px;
				box-shadow: 0 0 0 20px var(--white);
				background-color: var(--green);
			}
		}
		& > div:nth-child(2) {
			transform: translateX(160px) scale(-1);
		}
	}
</style>

