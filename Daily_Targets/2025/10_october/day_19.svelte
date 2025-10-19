<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--darkgreen: #1a4341;
		--green: #5a9f48;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color: var(--darkgreen);
		& > div {
			position: absolute;
			height: 30px;
			width: 130px;
			background-color: var(--green);
			translate: 0px 50px;
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				translate: -100px -20px;
				aspect-ratio: 1;
				background-color: var(--darkgreen);
				box-shadow:
					0 0 0 30px var(--green),
					230px -130px var(--darkgreen),
					230px -130px 0 30px var(--green);
				border-radius: 50%;
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 150px;
				background-color: var(--darkgreen);
				translate: -150px -70px;
				box-shadow:
					50px -30px var(--darkgreen),
					100px -30px var(--darkgreen),
					280px -30px var(--darkgreen),
					130px -30px var(--green);
			}
		}
	}
</style>
