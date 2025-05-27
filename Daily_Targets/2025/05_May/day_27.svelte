<div class="main">
	<div>
		<div></div>
	</div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #5aa4b7;
		--white: #ebf6f0;
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
		& > div:nth-child(1) {
			position: absolute;
			height: 210px;
			width: 180px;
			overflow: hidden;
			transform: translate(-50px);
			& > div {
				position: absolute;
				height: 60px;
				width: 180px;
				background-color: var(--white);

				&:before {
					position: absolute;
					content: '';
					height: 50px;
					width: 150px;
					background-color: var(--blue);
					border-top-left-radius: 30px;
					transform: translate(30px, 30px);
				}
				&:after {
					content: '';
					position: absolute;
					height: 180px;
					width: 60px;
					border-top-left-radius: 30px;
					background-color: var(--white);
					transform: translate(120px, 30px);
				}
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--blue);
			border-radius: 50%;
			transform: translate(90px, -55px);
			box-shadow:
				0 110px var(--blue),
				0 0 0 30px var(--white),
				0 110px 0 30px var(--white);
		}
	}
</style>
