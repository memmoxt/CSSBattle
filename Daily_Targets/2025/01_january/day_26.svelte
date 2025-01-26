<div class="main">
	<div></div>
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
		--red: #ac342e;
		--white: #ffffff;
		& > div {
			position: absolute;
			left: 0px;
			top: 0px;
			height: 300px;
			width: 185px;
			box-shadow: 215px 0 var(--red);
			background-color: var(--red);

			&:before {
				position: absolute;
				content: '';
				height: 30px;
				width: 160px;
				top: 135px;
				left: 120px;
				background-color: var(--white);
				box-shadow:
					160px -75px var(--white),
					160px 75px var(--white),
					-160px -75px var(--white),
					-160px 75px var(--white);
			}
		}
	}
</style>

