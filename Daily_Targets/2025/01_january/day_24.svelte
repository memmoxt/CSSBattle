<div class="main">
	<div><div><div></div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--white: #e0e7ff;
		--blue: #2d3464;
		--light_blue: #328fc1;
		background-color: var(--white);
		& > div:nth-child(1) {
			position: absolute;
			height: 184px;
			aspect-ratio: 1;
			left: 55px;
			border-radius: 50%;
			overflow: hidden;
			& > div {
				position: absolute;
				height: 184px;
				aspect-ratio: 1;
				background-color: var(--blue);
				border-radius: 50%;
				left: 105px;
				overflow: hidden;
				& > div {
					position: absolute;
					height: 92px;
					width: 184px;
					background-color: var(--light_blue);
				}
			}
		}
	}
</style>

