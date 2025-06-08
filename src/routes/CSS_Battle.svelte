<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f2eaa8;
		--red: #ee7667;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--yellow);
		& > div:nth-child(1) {
			height: 200px;
			aspect-ratio: 1;
			background-color: var(--red);
			border-radius: 50%;
			overflow: hidden;
			position: absolute;
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 200px;
				width: 60px;
				transform: translate(70px);
				background-color: var(--yellow);
			}
			&:after {
				width: 40px;
				transform: translate(80px) rotate(-90deg);
			}
		}

		& > div:nth-child(2) {
			height: 200px;
			aspect-ratio: 1;
			position: absolute;
            overflow: hidden;
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 20px;
				background-color: var(--red);
				box-shadow: 0 140px var(--red);
				transform: translate(90px, -20px);
			}
			&:after {
				transform: translate(160px, 60px) rotate(90deg);
				height: 80px;
				width: 20px;
			}
		}
	}
</style>
