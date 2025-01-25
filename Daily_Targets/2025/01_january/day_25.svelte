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
		--orange: #ea9a52;
		--blue: #435998;
		--white: #ffffff;
		background-color: var(--orange);
		& > div,
		& > div:after {
			height: 300px;
			width: 250px;
			background-color: transparent;
			box-shadow: 0 0 0 30px var(--blue);
			transform: translate(0px, -150px);
			border-radius: 200px/200px;
			&:before {
				position: absolute;
				content: '';
				height: 300px;
				width: 30px;
				background-color: var(--white);
				top: 150px;
				left: 110px;
			}
			&:after {
				position: absolute;
				content: '';
				transform: translate(0px, 300px);
			}
		}
	}
</style>
