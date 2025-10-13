<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #4a9a86;
		--yellow: #fae29e;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			position: absolute;
			height: 240px;
			width: 40px;
			background-color: var(--yellow);
			translate: -80px;
			&:before {
				content: '';
				position: absolute;
				translate: -10px 130px;
				box-shadow: 0 0 0 30px var(--yellow);
				height: 60px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--green);
			}
		}
		& > div:nth-child(2) {
			translate: 80px;
			transform: scaleY(-1);
		}
	}
</style>
