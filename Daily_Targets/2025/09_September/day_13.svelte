<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f1e1be;
		--dark: #240d29;
        background-color:var(--white);
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
			content: '';
			position: absolute;
			height: 50px;
			width: 30px;
			translate: 0px -100px;
			box-shadow:
				-70px 30px var(--dark),
				70px 30px var(--dark),
				-70px 170px var(--dark),
				-70px 160px var(--dark),
				70px 170px var(--dark),
				70px 160px var(--dark),
				0px 200px var(--dark),
				0px 190px var(--dark);
			background-color: var(--dark);
            &:before{
                content:'';
                position:absolute;
                height:20px;
                width:105px;
                background-color:var(--dark);
                translate:110px 115px;
                box-shadow: -295px 0px var(--dark);
            }
		}
	}
</style>
