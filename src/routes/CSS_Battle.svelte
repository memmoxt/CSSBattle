<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #9382e4;
		--blue: #b6ebe7;
		--black: #3f595e;
        background-color: var(--purple);
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
			width: 28px;
			background-color: var(--blue);
			position: absolute;
			translate: -126px -90px;
			box-shadow:
				70px 60px var(--blue),
				140px 120px var(--blue),
				210px 180px var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 28px;
				width: 55px;
				translate: 20px 32px;
				background-color: var(--blue);
				box-shadow:
					70px 60px var(--blue),
					140px 120px var(--blue),
					205px 180px var(--blue);
			}
			&:after {
				content: '';
				position: absolute;
				height: 28px;
				aspect-ratio: 1;
				background-color: var(--black);
				translate: 70px 32px;
				box-shadow:
					70px 60px var(--black),
					140px 120px var(--black);
			}
		}
	}
</style>
