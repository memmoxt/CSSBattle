<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #6cb3a9;
		--red: #d25b70;
		--yellow: #f6df96;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--red);

		& > div {
			position: absolute;
			height: 150px;
			width: 400px;
			background-color: var(--green);
			transform: translate(0px, 75px);
			/* opacity: 0.5; */

			&:before {
				content: '';
				position: absolute;
				height: 200px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				border-radius: 50%;
				transform: translate(100px, -100px);
			}

			&:after {
				content: '';
				position: absolute;
				height: 15px;
				width: 400px;
				background-color: var(--green);
				box-shadow:
					0 25px var(--green),
					0 50px var(--green),
					0 75px var(--green);
				transform: translate(-0px, 00px);
			}
		}
	}
</style>
