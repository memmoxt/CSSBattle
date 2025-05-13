<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --yellow:#E3CC9E;
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
        &>div{
            position:absolute;
            height:80px;
            aspect-ratio:1;
            background-color:var(--red);
            border-radius:50%;
            transform:translate(-80px);
            box-shadow:160px 0 var(--red);
            &:before{
                content:'';
                position:absolute;
                width:240px;
                aspect-ratio:1;
                border-radius:50%;
                transform:translate(0px,-80px);
                clip-path:polygon(0px 0px , 240px 0px, 240px 120px, 0px 120px);
                background-color:var(--red);
            }
            &:after{
                content:'';
                position:absolute;
                height:200px;
                width:40px;
                transform:translate(100px);
                background-color:var(--red);
            }
        }

	}
</style>
