<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #d86f45;
		--white: #ffffff;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color:var(--orange);
		& > div {
			height: 50px;
			width: 250px;
			background-color: var(--orange);
			box-shadow: 0 0 0 20px var(--white);
			&:before {
				content: '';
				position: absolute;
				translate: 100px -60px;
				box-shadow:
					0 0 0 20px var(--white),
					0 0 0 30px var(--orange);
				height: 170px;
				width: 50px;
				background-color: var(--orange);
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				width: 150px;
				background-color: var(--orange);
				translate: 50px 10px;
			}
		}
	}
</style>
