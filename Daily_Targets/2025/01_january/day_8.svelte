<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
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
		--red: #d95362;
		--blue: #2d3464;
		background-color: var(--red);
		& > div {
			height: 220px;
			aspect-ratio: 1;
			background-color: var(--blue);
			border-radius: 50%;
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				width: 150px;
				background-color: var(--red);
				top: 130px;
				left: 125px;
			}
			&:after {
				top: 100px;
				left: 155px;
				transform: rotate(-90deg);
				width: 90px;
			}
		}
	}
</style>

