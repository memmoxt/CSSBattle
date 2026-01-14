<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--magenta: #a82973;
		--pink: #ffd0fa;
        background-color: var(--magenta);
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
			height: 120px;
			width: 50px;
			background-color: var(--pink);
			translate: -145px;
			box-shadow:
				60px 0 var(--pink),
				230px 0 var(--pink),
				290px 0 var(--pink);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--pink);
				translate: 30px -60px;
				border-radius: 50%;
				box-shadow:
					230px 0px var(--pink),
					0 190px var(--pink),
					230px 190px var(--pink);
			}
		}
	}
</style>
