<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #ffffff;
		--blue: #243d83;
        background-color:var(--blue);
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
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--white);
			box-shadow:
				0 0 0 40px var(--blue),
				0 0 0 60px var(--white);
                &:before{
                content:'';
                position:absolute;
                height: 260px;
                width: 45.5px;
                background-color:var(--blue);
                translate: 38px -75px;
            }
            &:after{
                content:'';
                position:absolute;
                height:46px;
                width: 250px;
                background-color: var(--blue);
                translate: -66px 38px;
            }
		}

	}
</style>

