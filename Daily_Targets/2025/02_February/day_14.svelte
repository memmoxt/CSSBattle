<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #963032;
		--green: #75cf34;
        background-color:var(--green);
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
            height:40px;
            width:120px;
            background-color:var(--red);
            transform:translate(60px,-30px);
            &:before{
                content:'';
                position:absolute;
                height:25px;
                width:40px;
                transform:translate(10px, -20px);
                background-color:var(--red);
                box-shadow:60px 0 var(--red);
            }
        }
        &>div:nth-child(2){
            transform:translate(-60px, 30px) scale(-1) ;
        }
	}
</style>

