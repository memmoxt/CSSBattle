<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffcd;
		--blue: #6592cf;
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
		& > div {
			position: absolute;
			height: 180px;
			width: 280px;
			background-color: var(--blue);
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--blue);
				border-radius: 50%;
				transform: translate(-120px, 180px);
				box-shadow: 0 0 0 60px var(--white);
			}
			&:after {
				transform: translate(280px, -120px);
			}
		}
	}
</style>
