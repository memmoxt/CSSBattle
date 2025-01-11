<div class="main">
	<div></div>
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
		--dark: #2f5a76;
		--light: #7ea6dd;
        background-color:var(--dark);
		& > div {
			position: absolute;
			top: 70px;
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--dark);
			/* opacity: 50%; */
			border-radius: 50%;
			box-shadow: 0 0 0 30px var(--light);
			&:before {
				position: absolute;
				content: '';
				background-color: var(--dark);
				top: 20px;
				left: -40px;
				height: 70px;
				width: 70px;
			}
		}
		& > div:nth-child(1) {
			transform: translateY(100px) scaleY(-1);
		}
	}
</style>

