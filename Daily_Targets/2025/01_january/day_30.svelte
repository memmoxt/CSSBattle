<div class="main">
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
		box-sizing: content-box;
		--yellow: #fade8b;
		--green: #61a74e;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		--green: #5aed9c;
		--purple: #4b4d88;
		background-color: var(--green);
		& > div:nth-child(1) {
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--purple);
			border-radius: 50%;
		}
		& > div:nth-child(2),
		& > div:nth-child(3),
		& > div:nth-child(4),
		& > div:nth-child(5),
		& > div:nth-child(6) {
			position: absolute;
			content: '';
			height: 30px;
			width: 60px;
			background-color: var(--purple);
			border-radius: 50px/50px;
			left: 74px;
			top: 135px;
		}
		& > div:nth-child(3) {
			transform: translate(28px, -68px) rotate(45deg);
		}
		& > div:nth-child(4) {
			transform: translate(96px, -96px) rotate(90deg);
		}
		& > div:nth-child(5) {
			transform: translate(164px, -68px) rotate(-45deg);
		}
		& > div:nth-child(6) {
			transform: translate(192px, 0px);
		}
	}
</style>

