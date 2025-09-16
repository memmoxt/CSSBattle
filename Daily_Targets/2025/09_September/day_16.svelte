<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #152844;
		--red: #a34f46;
		--white: #ffffff;
        background-color:var(--red);
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
			position: absolute;
			background-color: var(--blue);
			height: 140px;
			width: 130px;
			translate: -135px -85px;
			box-shadow: 270px 0px var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 105px;
				width: 80px;
				background-color: var(--blue);
				translate: 160px 35px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 135px;
				width: 185px;
				translate: 0px 170px;
				background-color: var(--blue);
				box-shadow: 215px 0px var(--blue);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 60px;
			width: 30px;
			background-color: var(--white);
			translate: -165px 45px;
			box-shadow: 330px 0px var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 20px;
				background-color: var(--blue);
				translate: -20px -30px;
                box-shadow:380px 0px var(--blue);
			}
		}
	}
</style>
