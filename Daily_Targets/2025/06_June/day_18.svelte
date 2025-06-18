<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fade8b;
		--red: #d24444;
		background-color: var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 220px;
			width: 110px;
            background-color: var(--red);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 70px;
				top: 80px;
				box-shadow: 0 90px var(--yellow);
				background-color: var(--yellow);
			}
		}
	}
</style>
