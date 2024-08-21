<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #8baddb;
		--black: #000000;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			border-radius: 50%;
			transform: translateY(-40px);
            height:120px;
            aspect-ratio:1;
            background-color:var(--black);
            z-index: 2;
            clip-path:polygon(0 0 , 120px 0px, 120px 61px, 0px 61px);
		}
		& > div:nth-child(2),
		& > div:nth-child(3) {
			position: absolute;
			border-radius: 50%;
			border-top: 60px solid var(--black);
			border-right: 60px solid transparent;
			border-bottom: 60px solid transparent;
			border-left: 60px solid transparent;
			transform: translate(-50%, -40px) rotate(-225deg);
            z-index:1;
		}
		& > div:nth-child(3) {
			transform: translate(50%, -40px) rotate(225deg);
		}
		& > div:nth-child(4) {
			position: absolute;
			height: 20px;
            border-radius:50%;
			aspect-ratio: 1;
			background-color: var(--black);
			transform: translate(-30px,43px);
            box-shadow:60px 0px 0 var(--black);
		}
	}
</style>

