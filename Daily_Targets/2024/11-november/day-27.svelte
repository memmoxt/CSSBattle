<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #c0d6e7;
		--red: #d95362;
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
		& > div {
			height: 230px;
			width: 230px;
			background-color: var(--red);
            clip-path:polygon( 115px 0px, 230px 230px, 0px 230px);
            &:before{
                position:absolute;
                content:'';
                background-color:var(--blue);
                height:40px;
                width:250px;
                top:130px;
            }
		}
	}
</style>

