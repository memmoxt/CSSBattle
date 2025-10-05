<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #ffffff;
		--blue: #4763b1;
        background-color: var(--white);
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
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				width: 20px;
				background-color: var(--blue);
				translate: -130px -50px;
				box-shadow: 300px 0px var(--blue);
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				width: 260px;
				background-color: var(--blue);
				translate: -100px -80px;
				box-shadow: 0px 200px var(--blue);
			}
		}
	}
</style>
