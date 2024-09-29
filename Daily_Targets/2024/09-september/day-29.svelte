<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --white:#f0f0f0;
        --yellow:#eac049;
        --red:#e05947;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        flex-wrap: wrap-reverse;
        flex-direction: column;
        &>div{
            height:100px;
            aspect-ratio:1;
            background-color:var(--red);
            &:before{
                content:'';
                position:absolute;
                height:20px;
                width:100px;
                transform:translate(0px,20px);
                background-color:var(--white);
                box-shadow:0 40px var(--white) ;
            }
        }
        &>div:nth-child(2){
            background-color:var(--yellow);
            transform:rotate(90deg);
        }
	}
</style>

