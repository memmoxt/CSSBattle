<div class="main">
	<div class="forehead"></div>
	<div class="jaw"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f9e492;
		--black: #191919;
		--blue: #4f77ff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		/* background-color: var(--black); */
		& > .forehead {
			height: 100px;
			width: 120px;
			border-radius: 60px 60px 10px 10px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(15px, 53px);
				background-color: var(--black);
				box-shadow: 50px 0px 0px var(--black);
			}
		}
		& > .jaw {
			height: 30px;
			width: 80px;
			border-radius: 0 0 20px 20px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(30px, -10px);
				background-color: var(--black);
			}
			&:after {
				content: '';
				position: absolute;
				height: 10px;
				width: 10px;
				border-radius: 5px 5px 0 0;
				background-color: var(--black);
				transform: translate(35px, 20px);
				box-shadow:
					15px 0px 0px var(--black),
					-15px 0px 0px var(--black);
			}
		}
	}
</style>
