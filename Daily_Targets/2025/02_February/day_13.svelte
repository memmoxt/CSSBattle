<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #183539;
		--blue: #00b0c8;
		background-color: var(--blue);
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
			height: 240px;
			width: 120px;
			background-color: var(--green);
			/* opacity: 0.5; */
			transform: translate(-50px);
			&:before {
				content: '';
				position: absolute;
				height: 120px;
				width: 40px;
				background-color: var(--green);
				transform: translate(120px, 60px);
			}
		}
		& > div:nth-child(2) {
			transform: translate(50px) scale(-1);
		}
	}
</style>
