<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #4f77ff;
		--white: #e0e7ff;
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
		& > div:nth-child(1) {
			height: 280px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--blue);
			opacity: 1;
			&:before,
			&:after {
				position: absolute;
				content: '';
				background-color: var(--white);
			}
			&:before {
				top: 50px;
				left: 100px;
				border-radius: 50%;
				height: 200px;
				aspect-ratio: 1;
			}
			&:after {
				top: 110px;
				left: 264px;
				height: 80px;
				width: 100px;
				background-color: var(--white);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 180px;
			aspect-ratio: 1;
			background-color: var(--blue);
			opacity: 1;
			border-radius: 50%;
			&:before,
			&:after {
				position: absolute;
				content: '';
			}
			&:before {
				height: 100px;
				aspect-ratio: 1;
				border-radius: 50%;
				top: 40px;
				left: 40px;
				background-color: var(--white);
			}
			&:after {
				height: 40px;
				width: 50px;
				background-color: var(--white);
				top: 70px;
				left: 133px;
			}
		}
	}
</style>
