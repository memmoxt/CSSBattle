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
		box-sizing: content-box;
		--red: #d95362;
		--white: #c0d6e7;
		--blue: #2d3464;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--red);
		& > div:nth-child(1) {
			position: absolute;
			height: 114px;
			aspect-ratio: 1;
			background-color: var(--blue);
			transform: rotate(-45deg);
            z-index:10;
		}
		& > div:nth-child(2),
		div:nth-child(3) {
			position: absolute;
			height: 100px;
			aspect-ratio: 2/1;
			background-color: var(--red);
			clip-path: polygon(0 0, 200px 0px, 100px 100px);
			transform: translate(-150px, 40px);
            z-index:11;
		}
		& > div:nth-child(3) {
			transform: translate(150px, 40px);
		}
		& > div:nth-child(4) {
			position: absolute;
			background-color: var(--white);
			height: 200px;
			aspect-ratio: 1;
			transform: translateY(-81px) rotate(-45deg);
            box-shadow: -115px 115px var(--white);
		}
	}
</style>
