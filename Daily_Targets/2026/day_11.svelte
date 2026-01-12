<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5aa4b7;
		--white: #f9eaf1;
		--black: #4c455b;
        background-color: var(--blue);
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
			height: 130px;
			width: 120px;
			translate: -40px 40px;
			background-color: var(--black);
			box-shadow: 80px -80px var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 10px;
				width: 40px;
				background-color: var(--blue);
				translate: 80px;
				box-shadow:
					0px 10px var(--white),
					0px 20px var(--blue),
					0 30px var(--black),
					0 40px var(--blue);
			}
		}
	}
</style>
