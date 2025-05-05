<div class="main">
	<div class="circle"></div>
	<div class="circle"></div>
	<div class="long"></div>
	<div class="short"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --red:#D95F5B;
        --white:#E3DCD1;
        background-color: var(--white);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        &>.circle{
            position:absolute;
            height:80px;
            width:40px;
            background-color:transparent;
            transform:translate(-50px,-30px);
            overflow: hidden;
            &:before{
                content:'';
                position:absolute;
                height:40px;
                aspect-ratio:1;
                border-radius:50%;
                transform:translate(20px,20px);
                background-color:transparent;
                box-shadow:0 0 0 20px var(--red);
            }
        }
        &>.circle:nth-child(2){
            transform:translate(50px, 30px) scale(-1);
        }
        &>.long{
            position:absolute;
            height:20px;
            width:160px;
            background-color: var(--red);
            transform:translate(50px,-60px);
            box-shadow:-100px 120px var(--red);
        }
        &>.short {
            position:absolute;
            height:20px;
            width:60px;
            background-color: var(--red);
        }
	}
</style>

