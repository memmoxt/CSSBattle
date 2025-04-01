<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #436f9b;
		--orange: #e38f66;
        background-color: var(--blue);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;

		& > div {
			height: 80px;
			width: 30px;
			background-color: var(--orange);
            position: absolute;
			/* opacity: 0.5; */
			&:before,
			&:after {
				position: absolute;
				content: '';
				height: 30px;
				width: 100px;
				background-color: var(--orange);
				transform: translate(-70px, 100px);
			}
			&:after {
				height: 30px;
				width: 30px;
				background-color: var(--orange);
				transform: translate(-70px, 50px);
			}
		}
		& > div:nth-child(1) {
			transform: scale(-1);
		}
	}
</style>

