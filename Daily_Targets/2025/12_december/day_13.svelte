<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #a33e52;
		--white: #d9d9d9;
		--brown: #482222;
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
		& > div {
			height: 200px;
			width: 300px;
			background-color: var(--red);
            border: 30px solid var(--brown);
			&:before {
				content: '';
				position: absolute;
                height:30px;
                width: 240px;
                background-color: var(--white);
                box-shadow: 0 110px var(--white);
			}
            &:after{
                content:'';
                position:absolute;
                height: 200px;
                width: 30px;
                background-color: var(--white);
                translate: -60px -30px;
                box-shadow: 330px 0px var(--white);
            }
		}
	}
</style>
