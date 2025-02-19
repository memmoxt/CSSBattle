<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #d95362;
		--white: #fdffe9;
		background-color: var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 220px;
			width: 80px;
			background-color: var(--white);
			/* opacity: 0.5; */
			position: absolute;
			left: 125px;
			&::before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				left: 100px;
				box-shadow:
					0 85px var(--white),
					0 170px var(--white);
			}
		}
	}
</style>
