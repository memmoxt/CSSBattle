<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --yellow:#ebe77e;
        --red:#de817e;
        background-color:var(--yellow);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: start;
		align-items: center;
		position: absolute;
        &>div:nth-child(2){
            height:140px;
            width:100px;
            background-color:var(--red);
        }
        &>div:nth-child(1){
            border-top: 70px solid var(--yellow);
            border-right: 60px solid var(--red);
            border-bottom: 70px solid var(--yellow);
            border-left: 90px solid var(--yellow);
        }
        &>div:nth-child(3){
            border-top: 70px solid var(--red);
            border-right: 60px solid var(--yellow);
            border-bottom: 70px solid var(--red);
            border-left: 0px solid var(--red);

        }

	}
</style>

