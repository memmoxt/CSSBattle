<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --yellow:#F4DA64;
        --blue:#243D83;
        --red:#D95F5B;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        &>div:nth-child(1), div:nth-child(2){
            --color:var(--blue);
            position:absolute;
            height:40px;
            width:40px;
            background-color:var(--color);
            z-index:2;
            &:before{
                content:'';
                position:absolute;
                height:80px;
                width:40px;
                transform:translate(0px, 50px);
                background-color:var(--color);
                box-shadow:0px -140px var(--color);
            }
            &:after{
                content:'';
                position:absolute;
                height:40px;
                width:80px;
                background-color:var(--color);
                transform:translate(50px);
                box-shadow:-140px 0px var(--color);
            }
        }
        &>div:nth-child(2){
            --color:var(--red);
            transform:translate(0px,-10px);
            z-index:1;
        }

	}
</style>

