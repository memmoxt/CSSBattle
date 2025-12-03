<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #c8ad17;
		--black: #222222;
		--white: #eeeeee;
        background-color: var(--yellow);
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
			height: 20px;
			width: 80px;
			background-color: var(--white);
			translate: 0 -65px;
			box-shadow: 0 0 0 20px var(--black);
			&:before {
				content: '';
				position: absolute;
				height: 70px;
				width: 180px;
				background-color: var(--white);
				translate: -50px 40px;
				box-shadow: 0 0 0 20px var(--black);
				border-top-left-radius: 10px;
				border-top-right-radius: 10px;
			}
            &:after{
                content:'';
                position:absolute;
                height: 40px;
                width: 80px;
                background-color: var(--white);
                translate: 0 110px;
                box-shadow: 0 0 0 20px var(--black);
            }
		}
	}
</style>
