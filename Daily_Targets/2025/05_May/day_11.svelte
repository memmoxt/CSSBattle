<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #4c6b50;
		--yellow: #f7ec7d;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 300px;
			width: 400px;
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 160px;
				background-color: var(--green);
				transform: translate(120px, 120px);
				box-shadow:
					0 0 0 60px var(--yellow),
					0 0 0 120px var(--green);
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 160px;
				background-color: var(--yellow);
				transform: translate(120px, 120px);
				box-shadow:
					0 0 0 60px var(--green),
					0 0 0 120px var(--yellow);
				clip-path: polygon(80px -120px, 280px -120px, 280px 180px, 80px 180px);
			}
		}
	}
</style>

