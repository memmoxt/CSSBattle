<div class="main">
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #2d3464;
		--red: #d95362;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 60px;
			aspect-ratio: 1;
			position: absolute;
			background-color: transparent;
			overflow: hidden;
			& > div {
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--blue);
				/* opacity: 0.5; */
				border-radius: 50%;
				transform: translate(50%, 50%);
				box-shadow: 0 0 0 30px var(--red);
			}
		}
		& > div:nth-child(1) {
			transform: translate(-120px, 120px);
		}
		& > div:nth-child(2) {
			transform: translate(-60px, 90px) rotate(180deg);
		}
		& > div:nth-child(3) {
			transform: translate(-30px, 30px) rotate(0deg);
		}
        &>div:nth-child(4){
			transform: translate(30px, 30px) rotate(90deg);
        }
        &>div:nth-child(5){
			transform: translate(60px, 90px) rotate(-90deg);
        }
        &>div:nth-child(6){
			transform: translate(120px, 120px) rotate(90deg);
        }
	}
</style>

