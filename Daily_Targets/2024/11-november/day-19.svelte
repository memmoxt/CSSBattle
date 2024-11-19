<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #e0e7ff;
		--blue: #4f77ff;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 120px;
			border-radius: 50%;
			left: 64px;
			aspect-ratio: 1;
			background-color: var(--white);
			box-shadow: 0 0 0 40px var(--blue);
			&:before {
				position: absolute;
				content: '';
				top: 35px;
				left: -50px;
				height: 50px;
				width: 212px;
				background-color: var(--white);
			}
		}
		& > div:nth-child(2) {
			transform: translateX(152px);
		}
	}
</style>

