<div class="main">
	<div>
        <div></div>
    </div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #b0c1f0;
		--blue: #3e5aa9;
		background-color: var(--white);
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
			height: 100px;
			width: 380px;
			clip-path: polygon();
			overflow: hidden;
			& > div {
				position: absolute;
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--white);
				transform: rotate(45deg);
				translate: 130px -10px;
				box-shadow:
					0 0 0 30px var(--blue),
					0 0 0 40px var(--white),
					0 0 0 70px var(--blue);
				&:before {
					position: absolute;
					content: '';
					height: 20px;
					width: 180px;
					transform: rotate(-45deg);
					translate: -30px 50px;
					background-color: var(--blue);
				}
			}
		}
	}
</style>
