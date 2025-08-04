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
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--red: #d94e4e;
		--yellow: #ebe77e;
        background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;

		& > div:nth-child(1),
		& > div:nth-child(2) {
			height: 240px;
			width: 60px;
			background-color: var(--red);
			translate: -140px;
			border-top-right-radius: 25px;
			border-bottom-right-radius: 25px;
			border-top-left-radius: 35px;
			border-bottom-left-radius: 35px;
			box-shadow: 280px 0 var(--red);
			z-index: 5;
		}
		& > div:nth-child(2) {
			position: absolute;
			box-shadow:
				280px 0 0 20px var(--yellow),
				0px 0 0 20px var(--yellow);
			z-index: 2;
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 40px;
			width: 380px;
			background-color: var(--red);
			z-index: 6;
		}
        &>div:nth-child(4){
            position:absolute;
            background-color:var(--yellow);
            height:80px;
            width:380px;
        }
	}
</style>

