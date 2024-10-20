<div class="main">
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --green:#0b2429;
        --yellow:#f3ac3c;
        --gold:#998235;
        background-color:var(--green);

	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div{
            height:90px;
            width:130px;
            background-color:var(--yellow);
            border-radius:50px/50px;
            &:before{
                content:'';
                position:absolute;
                height:85px;
                width:90px;
                background-color:var(--gold);
                top:0;
                left:155px;
                box-shadow:0 215px 0 0 var(--gold);
            }
        }
	}
</style>

