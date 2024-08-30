<div class="main">
	<div></div>
	<div></div>
	<div></div>
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
		box-sizing: border-box;
		--yellow: #f9b140;
		--blue: #8cd5f5;
		--green: #708e31;
		--red: #ad4646;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--red);
			/* opacity: 30%; */
			border-radius: 50%;
			transform-origin: bottom;
			transform: translate(0, -30px);
		}
		& > div:nth-child(6) {
			transform: translate(0, -30px) rotate(60deg);
		}

		& > div:nth-child(2) {
			transform: translate(0, -30px) rotate(120deg);
		}
		& > div:nth-child(3) {
			transform: translate(0, -30px) rotate(180deg);
		}
		& > div:nth-child(4) {
			transform: translate(0, -30px) rotate(240deg);
		}
		& > div:nth-child(5) {
			transform: translate(0, -30px) rotate(-60deg);
		}
		& > div:nth-child(7) {
			height: 30px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			transform: translate(0);
            z-index:2;
		}
		& > div:nth-child(1) {
			height: 100px;
			width: 15px;
			border-radius: 0;
			transform: translateY(100px) translateX(1px);
			background-color: var(--green);
		}
	}
</style>

