<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --red:#AC474B;
        --white:#ffffff;
        background-color:var(--red);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        &>div{
            position:absolute;
            height:20px;
            aspect-ratio:1;
            background-color:var(--red);
            /* opacity:0.5; */
            transform:translate(-15px , -80px);
            border-radius:50%;
            border-bottom-right-radius: 0%;
            box-shadow: 0 0 0 10px var(--white);
            &:before{
                content:'';
                position:absolute;
                height:60px;
                aspect-ratio:1;
                background-color:var(--white);
                transform:translate(-45px, 50px);
                box-shadow:0 80px var(--white);
            }
        }
        &>div:nth-child(2){
            transform: translate(15px ,-80px) scaleX(-1);
        }
	}
</style>
