<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --blue:#243d83;
        --sky:#6592cf;
	}
	.main {
        height:300px;
        width:400px;
		display: flex;
		justify-content: center;
		align-items: end;
        overflow:hidden;
        position: absolute;
        background:var(--blue);
        &>div{
            position:absolute;
            height:102px;
            width:80px;
            &:before{
                content:'';
                position:absolute;
                height:80px;
                width:80px;
                border-radius:50%;
                transform:translate(0px,-48%);
            }
        }
        &>div:nth-child(even){
            background-color:var(--blue);
            &:before{
                background-color:var(--blue);
            }
        }
        &>div:nth-child(odd){
            background-color:var(--sky);
            &:before{
                background-color:var(--sky);
            }
        } 
        &>div:nth-child(5){
            transform:scale(1.5) translateY(17px);
        }

        &>div:nth-child(4){
            transform:scale(2) translateY(25px);
        }

        &>div:nth-child(3){
            transform:scale(2.5) translateY(29.5px);
        }

        &>div:nth-child(2){
            transform:scale(3) translateY(33px);
        }

        &>div:nth-child(1){
            transform:scale(3.5) translateY(35px);
        }
	}
</style>
