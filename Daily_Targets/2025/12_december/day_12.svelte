<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #63b476;
		--blue: #243d83;
		--dark: #000e37;
		--white: #ffffff;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			content: '';
			position: absolute;
			height: 30px;
			width: 50px;
			background-color: var(--white);
			translate: 95px 0px;
			border-radius: 50px;
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 180px;
				translate: -160px -35px;
				border-radius: 50px;
				background-color: var(--blue);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 100px;
				background-color: var(--dark);
				translate: -160px -35px;
				border-radius: 50%;
			}
		}
		& > div:nth-child(2) {
			height: 30px;
			width: 95px;
			background-color: var(--white);
			translate: -73px;
			border-radius: 50px;
		}
	}
</style>

