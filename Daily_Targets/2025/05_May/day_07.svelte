<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --white:#C0D6E7;
        --marineblue:#2D3464;
        --teal:#5AA4B7;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        &>div{
            position:absolute;
            border-top: 0px solid var(--teal);
            border-right: 200px solid var(--marineblue);
            border-bottom: 300px solid var(--teal);
            border-left: 200px solid var(--marineblue);
            &:before{
                position:absolute;
                content:'';
                border-top: 300px solid var(--white);
                border-right: 200px solid transparent;
                border-bottom: 0px solid transparent;
                border-left: 200px solid transparent;
                transform:translate(-200px);
            }
        }
	}
</style>

