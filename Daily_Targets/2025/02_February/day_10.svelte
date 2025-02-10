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
		--blue: #328fc1;
		--white: #ffffff;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1),
		& > div:nth-child(2) {
			transform: translateX(-95px);
			height: 150px;
			width: 100px;
			background-color: var(--blue);
			&:before {
				position: absolute;
				content: '';
				height: 200px;
				aspect-ratio: 1;
				left: -140px;
				top: -25px;
				border-radius: 80px/100px;
				background-color: var(--white);
			}
		}
		& > div:nth-child(2) {
			transform: translate(95px) scale(-1);
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 50px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--blue);
		}
	}
</style>
