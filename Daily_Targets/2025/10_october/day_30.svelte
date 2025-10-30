<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #00b1d4;
		--black: #000000;
		--yellow: #fade8b;
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
			position: absolute;
			height: 48px;
			width: 348px;
			border-radius: 50px / 50px;
			background-color: var(--blue);
			translate: 0px -100px;
			box-shadow: 0px 0px 0 16px var(--black);

			&:before {
				content: '';
				position: absolute;
				height: 248px;
				width: 48px;
				border-radius: 50px / 50px;
				background-color: var(--blue);
                box-shadow: 0px 0px 0 16px var(--black);
			}
            &:after{
                content:'';
                position:absolute;
                height: 48px;
                aspect-ratio:1;
                background-color: var(--yellow);
                border-top-right-radius:50px;
                border-top-left-radius:50px;
                border-bottom-left-radius:50px;
                box-shadow: 0px 0px 0 16px var(--black);
            }
            
		}
	}
</style>
