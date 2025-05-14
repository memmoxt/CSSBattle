<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #243d83;
		--lightblue: #5aa4b7;
        background-color:var(--blue);
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
            border-top: 0px solid transparent;
            border-right: 80px solid transparent;
            border-bottom: 80px solid var(--lightblue);
            border-left: 80px solid transparent;
            transform:translate(0px, -80px);
            &:before{
                content:'';
                position:absolute;
                height:80px;
                width:160px;
                background-color:var(--lightblue);
                transform:translate(-80px,80px);
            }
            &:after{
                content:'';
                position:absolute;
                height:80px;
                aspect-ratio:1;
                background-color:var(--blue);
                border-radius:50%;
                transform:translate(-120px,80px);
                box-shadow: 160px 0 var(--blue), 80px 40px 0 40px var(--lightblue);
            }
        }
	}
</style>
