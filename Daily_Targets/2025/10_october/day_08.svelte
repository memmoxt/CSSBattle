<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #48bf7d;
		--dark: #0b2429;
        background-color: var(--green);
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
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--dark);
			border-radius: 50%;
			translate: -45px 0px;
			box-shadow:
				90px 0px var(--dark),
				0px 75px var(--dark),
				90px 75px var(--dark),
				90px -75px var(--dark),
				-0px -75px var(--dark);
            &:before{
                content:'';
                position:absolute;
                height: 40px;
                width: 170px;
                background-color: var(--dark);
                translate: -150px -75px;
                box-shadow: 260px 0px var(--dark), 260px 150px var(--dark), 0px 150px var(--dark);
            }
		}
	}
</style>
