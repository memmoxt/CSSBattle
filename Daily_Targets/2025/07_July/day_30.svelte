<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #48bf7d;
		--yellow: #feff58;
		--blue: #3e5aa9;
        background-color:var(--green);
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
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--green);
			border-radius: 50%;
			translate: -15px;
			box-shadow: 0 0 0 30px var(--yellow);

			&:before {
				content: '';
				position: absolute;
				height: 200px;
				width: 30px;
				background-color: var(--blue);
				box-shadow:
					30px 0px var(--yellow),
					60px 0px var(--yellow);
				translate: 70px -30px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 200px;
				width: 70px;
				background-color: var(--green);
                translate:130px -60px;
			}
		}
	}
</style>
