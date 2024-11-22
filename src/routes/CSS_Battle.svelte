<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #984842;
		--white: #ecd5e4;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 90px;
			width: 180px;
			background-color: var(--red);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--red);
				top: 0;
				left: 0;
				height: 30px;
				width: 60px;
				box-shadow:
					340px 0 0 0 var(--red),
					340px 270px 0 var(--red),
					0px 270px 0 var(--red);
			}
		}
	}
</style>
