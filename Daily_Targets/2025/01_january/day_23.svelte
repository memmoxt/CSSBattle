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
		--light_blue: #a1e6e4;
		--dark_blue: #2f5a76;
        background-color:var(--light_blue);
		& > div {
			height: 200px;
			width: 300px;
			background-color: var(--dark_blue);
			&:before {
				position: absolute;
				content: '';
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--light_blue);
				box-shadow:
					270px 0 var(--light_blue),
					0px 170px var(--light_blue),
					270px 170px var(--light_blue),
					30px 85px var(--light_blue),
					240px 85px var(--light_blue);
			}
			&:after {
				position: absolute;
				content: '';
				height: 80px;
				width: 180px;
				top: 110px;
				left: 110px;
				background-color: var(--light_blue);
			}
		}
	}
</style>

