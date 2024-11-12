<div class="main">
	<div>
        <div></div>
    </div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #9d92c8;
        --white:#f9ddc6;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--blue);
        &>div:nth-child(1){
            height:80px;
            aspect-ratio:1;
            transform:translate(20px,-58px);
            overflow:hidden;
            &>div{
                transform:translate(50%,50%);
                border-radius:100px;
                height:80px;
                box-shadow:0 0 0px 40px var(--white);
                aspect-ratio:1;
                background-color:var(--blue);
            }
        }
        &>div:nth-child(2),&>div:nth-child(2):before{
            position:absolute;
            height:126px;
            width:40px;
            bottom:42px;
            background-color:var(--white);
        }
        &>div:nth-child(2):before{
            content:'';
            transform:translate(0px,39px) rotate(90deg);
            height:120px;
        }
        
	}
</style>

