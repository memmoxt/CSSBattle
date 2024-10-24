<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f0f0f0;
		--red: #e05947;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 80px;
			width: 200px;
			background-color: var(--red);
			border-radius: 120px/50px;
            &:before{
                content:'';
                position:absolute;
                height:170px;
                width:40px;
                top:65px;
                left:180px;
                border-radius:50px/50px;
                background-color:var(--white);
                box-shadow:0 0 0px 15px var(--red);
            }
		}
	}
</style>

