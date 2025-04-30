<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        --orange:#F5E3B5;
        --red:#8D424D;
        overflow:hidden;
        background-color:var(--orange);
        &>div{
            position:absolute;
            height:120px;
            width:60px;
            background-color:var(--orange);
            border-radius:50px/50px;
            border-top-right-radius: 0;
            border-top-left-radius: 0;
            top:0;
            box-shadow:0px 60px 0 30px var(--red), 0 0 0 30px var(--red);
            /* opacity:0.5; */
            &:before{
                content:'';
                position:absolute;
                height:30px;
                aspect-ratio:1;
                border-radius:50%;
                background-color:var(--red);
                transform:translate(15px, 75px);
                box-shadow: 0 60px var(--orange);
            }
        }
	}
</style>
