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
        --black:#222222;
        --yellow:#f7ec7d;
        background-color:var(--yellow);
        &>div{
            height:190px;
            aspect-ratio:1;
            border-radius:50%;
            background-color:var(--black);
            &:before,&:after{
                content:'';
                position:absolute;
            }
            &:before{
                height:50px;
                width:250px;
                transform:translate(-30px,70px);
                background-color:var(--black);
            }
            &:after{
                height:90px;
                aspect-ratio:1;
                border-radius:50%;
                background-color:var(--yellow);
                transform:translate(50px,50px);
            }
        }

	}
</style>

