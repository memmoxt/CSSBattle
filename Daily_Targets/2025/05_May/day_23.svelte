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
		box-sizing: content-box;
		--light: #bfe33a;
		--dark: #5a9f48;
        background-color:var(--light);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 240px;
			aspect-ratio: 1;
			display: flex;
			justify-content: space-between;
			align-content:space-between;
            flex-wrap:wrap;
            gap:50px;
			& > div {
				position: relative;
				height: 80px;
				aspect-ratio: 1;
				background-color: var(--dark);
                &:before{
                    content:'';
                    position:absolute;
                    height:40px;
                    aspect-ratio:1;
                    background-color:var(--light);
                }
			}
            &>div:nth-child(1){
                transform:rotate(-180deg);
            }
            &>div:nth-child(2){
                transform:rotate(-270deg);
            }
            &>div:nth-child(3){
                transform:rotate(-90deg);
            }
		}
	}
</style>
