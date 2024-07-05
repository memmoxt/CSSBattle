<div class="main">
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
        --red:#B53733;
        --orange:#EA7457;
	}
	.main {
        height:300px;
        width:400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--red);
        &>div{
            background-color:var(--orange);
        }
        &>div:nth-child(1),&>div:nth-child(2){
            height:100px;
            width:50px;
            transform:translate(-150px,100px);
        }
        &>div:nth-child(2){
            transform:translate(-200px,-100px);
        }
        &>div:nth-child(3){
            position:absolute;
            height:250px;
            width:150px;
            transform:translate(75px,25px);
        }
        &>div:nth-child(4){
            position:absolute;
            height:100px;
            width:50px;
            transform:translate(175px,0px);
        }
	}
</style>

