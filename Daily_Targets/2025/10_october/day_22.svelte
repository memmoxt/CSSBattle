<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #d62e65;
		--white: #eeeeee;
        background-color: var(--red);
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
			height: 120px;
			width: 60px;
			background-color: var(--red);
			border-radius: 80px/ 80px;
            border-bottom-left-radius: 0px;
            border-bottom-right-radius: 0px;
			box-shadow: 0 0 0 30px var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 100px;
				background-color: var(--red);
				translate: -50px 20px;
			}
            &:after{
                content:'';
                position:absolute;
                height: 60px;
                width: 120px;
                background-color: var(--red);
                translate: -30px 110px;
            }
		}
		& > div:nth-child(2) {
			content: '';
			position: absolute;
			height: 80px;
			width: 120px;
			translate: 0px 50px;
			background-color: var(--white);
			border-radius: 50px / 50px;
            &:before{
                content:'';
                position:absolute;
                height: 20px;
                width: 60px;
                background-color: var(--red);
                translate: 30px 30px;
                border-radius: 50px / 50px;
            }
		}
	}
</style>
