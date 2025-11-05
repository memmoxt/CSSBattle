<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #0b2429;
		--blue: #a7c2fa;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color: var(--green);
		& > div {
			position: absolute;
			height: 40px;
			width: 360px;
			transform: translate(0px, -110px);
			box-shadow: 0 200px var(--blue);
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 260px;
				width: 40px;
				translate: 10px;
				box-shadow: 300px 0px var(--blue);
				background-color: var(--blue);
			}
            &:after{
                content:'';
                position:absolute;
                height:40px;
                width: 160px;
                background-color: var(--green);
                translate: 100px 200px;
            }
		}
	}
</style>
