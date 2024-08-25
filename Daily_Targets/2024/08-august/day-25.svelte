<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #d95f5b;
		--white: #e3dcd1;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
            /* opacity:50%; */
			background-color: var(--white);
			border-radius: 30% /50%;
			width: 170px;
			height: 100px;
			top: 96px;
			box-shadow: 0 0 0 30px var(--red);
            &:before{
                position:absolute;
                content:'';
                background-color:var(--white);
                /* background-color:black; */
                height:200px;
                width:115px;
                transform:translate(28px, -40px);
            }
		}
	}
</style>

