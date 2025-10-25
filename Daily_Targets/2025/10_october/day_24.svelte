<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #4f77ff;
		--white: #ffeff2;
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
			height: 50px;
			width: 50px;
			background-color: var(--white);
			box-shadow:
				-125px -75px var(--blue),
				-145px -95px 0px 20px var(--white),
				125px 75px var(--blue),
				145px 95px 0 20px var(--white);
                &:before{
                content:'';
                position:absolute;
                height: 40px;
                width: 40px;
                translate: -165px -115px;
                box-shadow: 340px 240px var(--blue);
                background-color: var(--blue);
            }
		}
	}
</style>
