<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #c06c88;
		--yellow: #f4da64;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		background-color: var(--red);
		& > div {
			position: absolute;
			height: 80px;
			width: 260px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 70px;
				aspect-ratio: 1;
				background-color: var(--red);
				border-radius: 50%;
				box-shadow: 0 0 0 45px var(--yellow);
				translate: 95px 5px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 26px;
				background-color: var(--yellow);
				translate: 117px -20px;
			}
		}
	}
</style>
