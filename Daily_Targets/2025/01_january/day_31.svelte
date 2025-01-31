
<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #c15965;
		--blue: #2f5a76;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		background-color: var(--blue);
		& > div {
			height: 140px;
			width: 200px;
			border-radius: 70px/70px;
			background-color: var(--blue);
			box-shadow: 0 0 0 40px var(--red);
			&:before {
				content: '';
				position: absolute;
				top: 110px;
				left: 160px;
				border-top: 10px solid transparent;
				border-right: 40px solid transparent;
				border-bottom: 60px solid var(--red);
				border-left: 40px solid transparent;
			}
			&:after {
				content: '';
				position: absolute;
				top: 210px;
				left: 160px;
				height: 60px;
				width: 80px;
				background-color: var(--blue);
			}
		}
	}
</style>
