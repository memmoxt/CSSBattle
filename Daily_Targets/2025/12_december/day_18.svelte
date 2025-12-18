<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f0cd48;
		--green: #1d7b47;
		--dark: #08331b;
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
			width: 190px;
			height: 210px;
			background-color: var(--green);
			&:before {
				content: '';
				position: absolute;
				height: 70px;
				aspect-ratio: 1;
				background-color: var(--dark);
				box-shadow:
					120px 70px var(--dark),
					0px 140px var(--dark);
			}
		}
	}
</style>
