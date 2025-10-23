<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--blue: #414b81;
		background-color: var(--yellow);
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
			position: absolute;
			height: 120px;
			width: 40px;
			background-color: var(--blue);
			translate: -60px 40px;
			box-shadow:
				60px -40px var(--blue),
				120px -80px var(--blue),
				120px 0px var(--blue),
				0px -80px var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 200px;
				background-color: var(--blue);
				translate: -20px 40px;
				box-shadow: 0px -80px var(--blue);
			}
		}
	}
</style>
