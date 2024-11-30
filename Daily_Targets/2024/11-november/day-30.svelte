<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--darkred: #8f3f4a;
		--red: #d96c7b;
		--white: #f3ead2;
        background-color:var(--white);
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
			height: 140px;
			width: 155px;
			background-color: var(--darkred);
			clip-path: polygon(1px 0, 44px 0, 95px 140px, 52px 140px);
			position: absolute;
            z-index: 2;
            /* opacity:0.5; */
		}
		& > div:nth-child(2) {
			background-color: var(--red);
			transform: scaleX(-1);
            z-index: 1;
		}
		& > div:nth-child(3) {
            z-index: 3;
            height:20px;
            position:absolute;
            top:125px;
            width:450px;
            background-color:var(--darkred);
            box-shadow:0 10px 0 0 var(--white);
		}
	}
</style>

