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
		--light: #6592cf;
		--dark: #243d83;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--dark);
		& > div {
			position: absolute;
			height: 200px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color:var(--light);
            overflow:hidden;
			& > div {
				position: absolute;
				height: 130px;
                transform:translate(110px,35px);
                border-radius:50%;
				aspect-ratio: 1;
				background-color: transparent;
                box-shadow:0 0 0 20px var(--dark);
			}
            &>div:nth-child(2){
                transform:translate(-40px,35px);
            }
            &>div:nth-child(3){
                transform:translate(35px,-40px);
            }
            &>div:nth-child(4){
                transform:translate(35px,110px);
            }
		}
	}
</style>
