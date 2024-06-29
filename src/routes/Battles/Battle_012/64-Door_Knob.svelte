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
		--blue: #5dbcf9;
		--black: #191919;
		--amber: #f2ad43;
		--yellow: #fff58f;
		--orange: #e08027;
		--brown: #824b20;
		background: var(--black);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-content: center;
		justify-items: center;
		align-items: center;
		& > div:nth-child(1) {
			position: absolute;
			height: 160px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--brown);
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 100px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--orange);
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 120px;
			aspect-ratio: 1;
			border-radius: 50%;
			border-top: 20px solid transparent;
			border-right: 20px solid transparent;
			border-bottom: 20px solid var(--yellow);
			border-left: 20px solid var(--yellow);
			transform: rotate(-45deg);
			background-color: transparent;
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--yellow);
				transform: translate(-5px, -5px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--yellow);
				transform: translate(65px, 65px);
			}
		}
	}
</style>
