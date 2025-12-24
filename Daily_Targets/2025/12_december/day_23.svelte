<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #dacfa3;
		--blue: #2d3464;
		--red: #d95362;
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
			height: 100px;
			width: 80px;
			background-color: var(--blue);
			box-shadow:
				0px -110px var(--blue),
				0px 110px var(--blue);
			&:before {
				content: '';
				position: absolute;
                aspect-ratio:1;
                height: 80px;
                background-color: var(--red);
                border-radius:50%;
                translate:-100px 10px;
                box-shadow: 200px 0px var(--red);
			}
		}
	}
</style>

