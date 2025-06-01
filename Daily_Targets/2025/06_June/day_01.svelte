<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --purple:#9076D8;
        --white:#FFFFFF;
        background-color:var(--purple);
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
            height:140px;
            width:60px;
            background-color:var(--purple);
            border-radius:50px/50px;
            box-shadow:0 0 0 30px var(--white);
            &:before{
                content:'';
                position:absolute;
                height:100px;
                aspect-ratio:1;
                background-color:var(--purple);
                transform:translate(-50px,-10px)
            }
            &:after{
                content:'';
                position:absolute;
                height:60px;
                aspect-ratio:1;
                background-color:var(--purple);
                border-radius:50%;
                box-shadow:0 0 0 30px var(--white);
            }
            
        }
	}
</style>

