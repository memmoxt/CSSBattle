<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --purple:#301e53;
        --violet:#766d94;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div:nth-child(1), &>div:nth-child(2){
            background-color:var(--violet);
            opacity:0.7;
            height:100px;
            aspect-ratio:1;
            transform:translate(-50%,-50%);
            &:before{
                content:'';
                position:absolute;
                height:50px;
                aspect-ratio:1;
                background-color:var(--purple);
                transform:translate(100%,100%);
            }
        }
        &>div:nth-child(2){
            transform:translate(50%,50%) scale(-1);
        }
	}
</style>
