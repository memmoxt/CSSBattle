<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #2f5a76;
		--yellow: #f5bb60;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 300px;
			width: 400px;
			background-color: var(--yellow);
			clip-path: polygon(0 0, 20px 0, 400px 219px, 400px 300px, 380px 300px, 0px 80.5px);
		}
		& > div:nth-child(2) {
			transform: scaleX(-1);
		}
	}
</style>
