<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--dark: #3f4869;
		--red: #de6b67;
        background-color: var(--dark);
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
			height: 290px;
			width: 210px;
			background-color: var(--red);
			border-radius: 105px / 105px;
			&:before {
				content: '';
				position: absolute;
				background-color: var(--red);
				height: 70px;
				width: 210px;
                translate:0px 110px;
                border-radius: 15px / 70px;
                box-shadow:0px 0px 0 40px var(--dark);
			}
		}
	}
</style>
