<div class="main">
	<div></div>
	<div class="top"><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #4c3ab3;
		--red: #d96e9f;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--purple);

		& > div:nth-child(1) {
			z-index: 2;
			position: absolute;
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--red);
			/* opacity: 0.5; */
			transform: translate(0px, -20px);
			border-radius: 50%;
			&:before {
				content: '';
				position: absolute;
				height: 146px;
				width: 71px;
				background-color: var(--red);
				transform: translate(49px, 14px);
				box-shadow: -130px 0 var(--red);
			}
			&:after {
				content: '';
				position: absolute;
				height: 115px;
				width: 10px;
				background-color: var(--purple);
				transform: translate(-50px, 14px);
				box-shadow: 130px 0 var(--purple);
			}
		}
	}

	.top {
		position: absolute;
		height: 100px;
		width: 200px;
		background-color: transparent;
		/* opacity: 0.5; */
		transform: translate(0px, -75px);
		overflow: hidden;

		& > div {
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--purple);
			border-radius: 50%;
			transform: translate(70px, 75px);
			box-shadow:
				0 0 0 31px var(--red),
				0 0 0 40px var(--purple),
				0 0 0 71px var(--red);
		}
	}
</style>
