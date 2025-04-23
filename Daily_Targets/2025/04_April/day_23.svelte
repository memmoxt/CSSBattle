<div class="main">
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --blue:#68D0DF;
        --purple:#9A5DCB;
        --white:#ffffff;
        background-color:var(--blue);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;

        &>div{
            height:160px;
            aspect-ratio:1;
            background-color:var(--white);
            
            position:absolute;
            &:before{
                content:'';
                position:absolute;
                height:40px;
                aspect-ratio:1;
                background-color:var(--purple);
                border-radius:50%;
                transform:translate(-50%,-50%);
                box-shadow:160px 160px var(--purple);
            }
            &:after{
                content:'';
                position:absolute;
                height:40px;
                width:80px;
                background-color:var(--purple);
                transform:translate(100%, -50%);
                box-shadow: -80px 160px var(--purple);

            }
        }

	}
</style>

