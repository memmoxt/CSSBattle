<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fff8ea;
		--green: #81d2b0;
		--red: #da6c8e;
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
			height: 50px;
			width: 120px;
			background-color: var(--red);
			box-shadow: 140px 70px var(--red);
			border-radius: 50px / 50px;
			translate: -70px -35px;
			&:before {
				content: '';
				position: absolute;
				height: 120px;
				width: 50px;
				translate: 140px -70px;
				border-radius: 50px / 50px;
				box-shadow: -70px 140px var(--green);
				background-color: var(--green);
			}
		}
	}
</style>
