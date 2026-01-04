<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #4c455b;
		--green: #8ab8b6;
		--white: #f3ead2;
        background-color: var(--black);
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
			height: 200px;
			width: 280px;
			background-color: var(--green);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--white);
				height: 20px;
				width: 60px;
				translate: 20px -20px;
				box-shadow:
					180px 0 var(--white),
					0px 220px var(--white),
					180px 220px var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				background-color: var(--white);
				height: 140px;
				width: 60px;
				translate: 20px 30px;
				box-shadow: 180px 0px var(--white);
			}
		}
	}
</style>
