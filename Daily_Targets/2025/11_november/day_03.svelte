<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #62306d;
		--orange: #e38f66;
        background-color: var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			position: absolute;
			height: 150px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--orange);
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 70px;
				background-color: var(--orange);
                box-shadow: 0px 291px var(--orange);
				translate: 40px -90px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 25px;
				aspect-ratio: 1;
				background-color: var(--orange);
				border-radius: 50%;
				translate: 40px -46px;
				box-shadow:
					22px 0px var(--orange),
					45px 0px var(--orange),
					0px 180px var(--orange),
					22px 180px var(--orange),
					45px 180px var(--orange),
					0px 234px var(--orange),
					22px 234px var(--orange),
					45px 234px var(--orange);
			}
		}
	}
</style>
