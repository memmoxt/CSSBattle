<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #0a6190;
		--light: #328fc1;
        background-color:var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 100px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--light);
		}
		& > div:nth-child(1) {
			transform: translate(-50px, -50px);
		}
        &>div:nth-child(2){
            transform:translate(50px,-50px);
        }

        &>div:nth-child(3){
            transform:translate(50px,50px);
        }

        &>div:nth-child(4){
            transform:translate(-50px,50px);
        }

        &>div:nth-child(5){
            transform:scale(1.5);
        }
	}
</style>

