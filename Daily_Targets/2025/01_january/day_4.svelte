<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		--blue: #2f5a76;
		--yellow: #f3ac3c;
        background-color:var(--blue);
		& > div {
			height: 190px;
			width: 120px;
			background-color: var(--blue);
			box-shadow: 0 0 0 20px var(--yellow);
            &:before{
                position:absolute;
                content:'';
                height:60px;
                width:360px;
                background-color:var(--yellow);
                left:20px;
                top:120px;
            }
		}
	}
</style>

