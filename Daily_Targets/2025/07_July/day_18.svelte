<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --pink:#F28BBB;
        --purple:#B03F7D;
        --red:#680039;
        background-color:var(--pink);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
        &>div{
            height:380px;
            width:300px;
            background-color:var(--pink);
            border-radius:250px/250px;
            box-shadow: 0 0 0 25px var(--purple);
            &:before{
                content:'';
                position:absolute;
                height:80px;
                width:135px;
                background-color:var(--red);
                translate:-25px 150px;
                box-shadow: 215px 0 var(--red);
            }
        }
	}
</style>
