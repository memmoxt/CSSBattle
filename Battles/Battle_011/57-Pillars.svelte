<div class="main">
	<div class="box">
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
		--yellow: #f9e492;
		--black: #191919;
		--blue: #4f77ff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--black);
		& > .box {
			position: absolute;
			height: 110px;
			aspect-ratio: 1;
			background-color: var(--blue);
			flex-wrap: wrap;
			display: flex;
			justify-content: space-between;
			align-content: space-between;
			& > div {
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--black);
                &:before{
                    content:'';
                    position:absolute;
                    height:45px;
                    aspect-ratio:1;
                    border-radius:50%;
                    background-color:var(--yellow);
                }
                &:after{
                    content:'';
                    position:absolute;
                    height:30px;
                    aspect-ratio:1;
                    border-radius:50%;
                    background-color:var(--blue);
                }
			}
			& > div:nth-child(1) {
				transform: translate(-20px, -20px) rotate(0deg);
			}
			& > div:nth-child(2) {
				transform: translate(70px, -20px) rotate(90deg);
			}
			& > div:nth-child(3) {
				transform: translate(-20px, 70px) rotate(-90deg);
			}
			& > div:nth-child(4) {
				transform: translate(70px, 70px) rotate(180deg);
			}
		}
	}
</style>

