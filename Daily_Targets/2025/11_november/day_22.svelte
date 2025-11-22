<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #328fc1;
		--yellow: #f5d6b4;
        background-color:var(--blue);
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
			height: 60px;
			width: 200px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 200px;
				translate: 0 -50px;
				background-color: var(--yellow);
				box-shadow: 0 130px var(--yellow);
			}
			&:after {
				content: '';
				position: absolute;
				height: 220px;
				aspect-ratio: 1;
				background-color: var(--blue);
				translate: -210px -80px;
				border-radius: 50%;
				box-shadow:
					0 0 0 30px var(--yellow),
					400px 0 var(--blue),
					400px 0 0 30px var(--yellow);
			}
		}
	}
</style>

