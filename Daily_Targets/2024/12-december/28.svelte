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
		--grey: #3f4869;
		--orange: #ea9a52;
		--red: #aa3440;
		--green: #61a74e;
        background-color:var(--grey);
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
		div:nth-child(2) {
			position: absolute;
			height: 60px;
			width: 180px;
			border-top-left-radius: 20px;
			border-top-right-radius: 20px;
			border-bottom-right-radius: 20px;
		}
		& > div:nth-child(1) {
			top: 60px;
			background-color: var(--orange);
		}
		& > div:nth-child(2) {
			bottom: 60px;
			transform: scaleY(-1);
			background-color: var(--red);
		}
		& > div:nth-child(3) {
			height: 60px;
			aspect-ratio: 1;
			transform: translateX(-60px);
			background-color: var(--green);
		}
	}
</style>

