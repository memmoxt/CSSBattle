<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --blue:#2D3464;
        --red:#D95362;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color:var(--blue);
		& > div {
			height: 20px;
			width: 120px;
			background-color: var(--red);
			translate: 0 60px;
			&:before ,&:after{
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--red);
                translate: -100% -100%;
                box-shadow: -40px -60px 0 20px var(--red),-80px -140px 0 20px var(--red);
			}
            &:after{
                transform: scaleX(-1);
                translate: 120px -40px;
            }
		}
	}
</style>
