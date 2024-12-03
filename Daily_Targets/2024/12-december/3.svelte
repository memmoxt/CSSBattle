<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5dbcf9;
		--white: #ffffff;
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
			height: 120px;
			width: 40px;
			background-color: var(--white);
			&:before {
				position: absolute;
				content: '';
                height:40px;
                width:120px;
                background-color:var(--white);
                top:40px;
                left:0px;
                box-shadow: 0 180px 0 0 var(--white);
			}
            &:after{
                position:absolute;
                content:'';
                height:300px;
                width:40px;
                background-color:var(--white);
                top:0;
                left:40px;
            }
		}
	}
</style>

