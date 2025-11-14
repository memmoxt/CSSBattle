<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #4f77ff;
		--yellow: #f0cd48;
		background-color: var(--blue);
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
			height: 280px;
			width: 60px;
			translate: -120px 50px;
			box-shadow: 240px 0 var(--yellow);
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 140px;
				background-color: var(--yellow);
				translate: 80px 20px;
				box-shadow:
					0 60px var(--yellow),
					0 120px var(--yellow),
					0 180px var(--yellow);
			}
		}
	}
</style>
