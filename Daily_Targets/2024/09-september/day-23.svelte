<div class="main">
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --brown:#5d3a3a;
        --green:#b5e0ba;
        background-color:var(--brown);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div{
            height:40px;
            width:200px;
            background-color:var(--green);

            &:before,&:after{
                content:'';
                position:absolute;
                height:60px;
                aspect-ratio:1;
                border-radius:50%;
                background-color:var(--green);
                transform: translate(70px ,-80px);
            }
            &:after{
                transform:translate(70px, 60px);
            }
        }
	}
</style>

