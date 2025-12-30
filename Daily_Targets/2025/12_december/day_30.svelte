<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--pink: #f8d2d1;
		--blue: #5aa4b7;
        background-color:var(--pink);
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
			height: 20px;
			width: 80px;
			background-color: var(--pink);
			translate: 0 -80px;
			box-shadow:
				0 0px 0 20px var(--blue),
				0 160px var(--pink),
				0 160px 0 20px var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				width: 20px;
				background-color: var(--pink);
				translate: -100px 50px;
				box-shadow:
					0 0 0 20px var(--blue),
					260px 0 var(--pink),
					260px 0 0 20px var(--blue);
			}
		}
	}
</style>
