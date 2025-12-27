<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing:content-box;
        --yellow:#F9DDC6;
        --purple:#594C94;
        background-color: var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        &>div{
            height: 120px;
            border-radius:50%;
            aspect-ratio:1;
            background-color: var(--purple); 
            &:before,&:after{
                content:'';
                position:absolute;
                height: 60px;
                aspect-ratio:1;
                background-color: var(--purple);
                border: 20px solid var(--yellow);
                translate: -40px 60px;
            }
            &:after{
                translate: 60px -40px;
            }
        }
        
	}
</style>

