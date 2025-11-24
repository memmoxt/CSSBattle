<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #d95362;
		--yellow: #fff9c0;
        background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(2) {
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			translate: -0px -40px;
			border-radius: 50%;
			background-color: var(--yellow);
			clip-path: polygon(0 0, 60px 0px, 60px 30px, 0px 30px);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--red);
				border-radius: 50%;
				translate: 20px 20px;
			}
		}
		& > div:nth-child(1) {
			translate: 0px 10px;
			height: 80px;
			width: 60px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				width: 450px;
				translate: -200px 80px;
				background-color: var(--yellow);
			}
		}
	}
</style>
