<div class="main">
    <div> </div>
    <div> </div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --red:#D95F5B;
        --black:#282828;
        background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        &>div:nth-child(1){
            position:absolute;
            height:60px;
            border-radius:50%;
            aspect-ratio:1;
            background-color:var(--red);
            box-shadow:0 0 0 20px var(--black);
            z-index:3;
            &:before{
                content:'';
                position:absolute;
                height:10px;
                width:6px;
                background-color:var(--black);
                transform:translate(27px,5px);
                box-shadow:0 40px var(--black);
            }
            &:after{
                content:'';
                position:absolute;
                height:6px;
                width:10px;
                background-color:var(--black);
                transform:translate(44px,27px);
                box-shadow:-40px 0px var(--black);
            }
        }
        &>div:nth-child(2){
            position:absolute;
            height:220px;
            width:60px;
            background-color:var(--black);
            border-radius:50px/50px;
            z-index:1;
        }
        
	}
</style>
