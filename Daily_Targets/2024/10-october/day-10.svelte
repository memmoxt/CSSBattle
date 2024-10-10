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
		box-sizing: border-box;
		--purple: #62306d;
		--red: #aa445f;
		--orange: #e38f66;
        /* background-color:var(--purple); */
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(odd) {
			position: absolute;
			height: 70px;
			aspect-ratio: 1;
			background-color: var(--orange);
			border-radius: 50%;
			transform: translate(-65px, -78px);
            opacity: 0.5;
		}
		& > div:nth-child(even) {
			position: absolute;
			height: 110px;
			width: 70px;
			transform: translate(0px, -78px);
			background-color: var(--red);
		}
		& > div:nth-child(3) {
			transform: translate(65px, -78px);
		}
		& > div:nth-child(4) {
			transform: translate(-65px, 77px);
		}
		& > div:nth-child(5) {
			transform: translate(0px, 77px);
		}
		& > div:nth-child(6) {
			transform: translate(65px, 77px);
		}
	}
</style>

