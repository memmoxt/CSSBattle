<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #30383f;
		--blue: #5aa4b7;
		--white: #ffffff;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--white);
			box-shadow: 0 0 0 20px var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 36px;
				width: 150px;
				translate: -45px 12px;
				background-color: var(--white);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 100px;
			transform: translate(100px);
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 36px;
				aspect-ratio: 1;
				translate: 32px 32px;
				border-radius: 50%;
				background-color: var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 36px;
				width: 100px;
				translate: 50px 32px;
				background-color: var(--white);
			}
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 100px;
			transform: scaleX(-1) translate(100px);
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 36px;
				aspect-ratio: 1;
				translate: 32px 32px;
				border-radius: 50%;
				background-color: var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 36px;
				width: 100px;
				translate: 50px 32px;
				background-color: var(--white);
			}
		}
	}
</style>
