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
		box-sizing: border-box;
		--orange: #ea9a52;
		--purple: #6255aa;
		--white: #ffffff;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color: var(--orange);
		& > div {
			--colort: var(--white);
			position: absolute;
			border-top: 60px solid transparent;
			border-right: 80px solid var(--colort);
			border-bottom: 60px solid transparent;
			border-left: 0px solid transparent;
		}
		& > div:nth-child(1) {
			position: absolute;
			height: 120px;
			aspect-ratio: 1;
			background-color: var(--purple);
		}
		& > div:nth-child(2) {
			translate: 20px;
		}
		& > div:nth-child(3) {
			transform: scaleX(-1);
			translate: -20px;
		}
		& > div:nth-child(4) {
			--colort: var(--purple);
			transform: translate(100px) scaleX(-1);
		}
		& > div:nth-child(5) {
			--colort: var(--purple);
			transform: translate(-100px);
		}
	}
</style>
