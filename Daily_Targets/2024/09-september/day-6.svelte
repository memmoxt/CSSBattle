<div class="main">
	<div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #328fc1;
		--black: #222222;
		--yellow: #fade8b;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		align-content: flex-start;
		& > div {
            position:absolute;
			background-color:var(--yellow);
			height: 72px;
			width: 145px;
			border-radius: 0px 0px 30px 0px;
			transform: rotate(30deg);
		}
        &>div:nth-child(2){
            transform:rotate(-30deg) scaleY(-1);
            z-index:2;
            &:before{
                height:10px;
                aspect-ratio:1;
                border-radius:50%;
                background-color:var(--yellow);
                content:'';
                position:absolute;
                transform:translate(121.5px ,17.5px);
                box-shadow: 0 0 0px 5px var(--black);
            }
        }
	}
</style>

