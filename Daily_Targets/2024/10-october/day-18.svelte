<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--brown: #191210;
		--red: #84271c;
        background-color:var(--brown);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
            position:relative;
			height: 240px;
			aspect-ratio: 1;
			background-color: var(--red);
			display: flex;
			& > div{
                position:absolute;
				height: 80px;
				aspect-ratio: 1;
				background-color: var(--brown);
                border-bottom-right-radius:40px;
			}
            &>div:nth-child(1){
                top:0;
                left:0;
            }
            &>div:nth-child(2){
                top:0;
                right:0;
                transform:scaleX(-1);
            }
            &>div:nth-child(3){
                bottom:0;
                left:0;
                transform:scaleY(-1);
            }
            &>div:nth-child(4){
                right:0;
                bottom:0;
                transform:scale(-1);
            }
		}
	}
</style>

