<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #282828;
		--white: #ffffff;
		--yellow: #f2a73b;
		--red: #ea3323;
		background-color: var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;

		padding-left: 20px;
		& > div:nth-child(1) {
			position: relative;
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--white);
			border-radius: 20px/20px;
			/* opacity: 0.5; */
			z-index: 3;
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 15px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--black);
				transform: translate(105px, 30px);
			}
		}
		& > div:nth-child(2) {
			aspect-ratio: 1;
			border-top: 40px solid transparent;
			border-right: 0px solid transparent;
			border-bottom: 40px solid transparent;
			border-left: 40px solid var(--yellow);
			/* opacity: 0.5; */
			z-index: 0;
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--red);
				transform: translate(-130px, -80px);
				border-radius: 50%;
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--red);
				transform: translate(-100px, -85px);
				border-radius: 50%;
			}
		}
		& > div:nth-child(3) {
			height: 10px;
			position: absolute;
			aspect-ratio: 1;
			background-color: var(--red);
			/* opacity: 50%; */
			border-radius: 50%;
			z-index: 0;
			transform: translate(-55px, -70px);
		}
	}
</style>

