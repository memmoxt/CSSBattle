<div class="main">
	<div><div></div></div>
	<div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #328fc1;
		--yellow: #f5d18c;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;

		& > div:nth-child(1) {
			overflow: hidden;
			height: 130px;
			width: 260px;
			background-color: transparent;
			display: flex;
			transform: translateY(-15px);
			justify-content: center;
			align-items: center;
			& > div {
				height: 260px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(0%, 65px);
				background-color: var(--blue);
			}
		}
		& > div:nth-child(2), div:nth-child(3) {
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			border-radius: 50%;
			transform: translate(-90px, 50px);
			background-color: var(--yellow);
			box-shadow: 0 0 0px 10px var(--blue);
		}
        &>div:nth-child(3){
            transform:translate(90px,50px);
            box-shadow: 0 0 0px 10px var(--blue), -90px 0 0px 20px var(--yellow);
        }
	}
</style>

