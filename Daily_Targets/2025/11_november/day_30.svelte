<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #e38f66;
		--white: #f7f3d7;
        background-color: var(--orange);
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
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--white);

			&:before {
				content: '';
				position: absolute;
				height: 70px;
				aspect-ratio: 1;
				background-color: var(--white);
                translate:-70px 0px;
                transform:translate(0px , 35px) rotate(-45deg) ;
                box-shadow: 149px 149px var(--white);
			}

            &:after {
                content:'';
                position: absolute;
                height: 70px;
                aspect-ratio:1;
                background-color: var(--white);
                translate: -140px 35px;
                box-shadow: 350px 0px var(--white);
            }
		}
	}
</style>
