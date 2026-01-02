<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --yellow:#F7CB71;
        --brown:#7C3219;
        --orange:#8B4524;
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
        &>div:nth-child(1),div:nth-child(2){
            position:absolute;
            height: 160px;
            width: 40px;
            background-color: var(--orange);
            transform: rotate(-45deg);
            translate: -80px;
            &:before{
                content:'';
                position:absolute;
                height:160px;
                width: 40px;
                background-color: var(--orange);
                transform: rotate(90deg);
            }
            &:after{
                content:'';
                position:absolute;
                height: 40px;
                aspect-ratio:1;
                background-color: var(--yellow);
                translate: 0px 60px;
            }
        }
        &>div:nth-child(2){
            translate:80px;
            background-color: var(--brown);
            &:before{
                background-color: var(--brown);
            }
        }
	}
</style>
