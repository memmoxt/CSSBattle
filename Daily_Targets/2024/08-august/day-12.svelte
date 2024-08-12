<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --green:#4a9a86;
        --yellow:#fae29e;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
       &>div{
            transform:translate(10px,5px);
            height:160px;
            width:80px;
            background-color:var(--yellow);
            &:before{
                content:'';
                position:absolute;
                background-color:var(--yellow);
                height:80px;
                width:40px;
                transform:translate(-40px,0px);
            }
            &:after{
                content:'';
                position:absolute;
                background-color:var(--green);
                border-radius:50%;
                height:80px;
                aspect-ratio:1;
                transform:translate(-100%,-50%);
            }
        } 
	}
</style>

