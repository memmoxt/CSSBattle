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
		--yellow: #fade8b;
		--red: #c3463d;
		--blue: #5dbcf9;
        background-color:var(--yellow);
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
			top: 60px;
			left: 34px;
			height: 180px;
			width: 140px;
			background-color: var(--blue);
		}
		& > div:nth-child(2) {
			left: 226px;
		}

		& > div:nth-child(3),
		div:nth-child(4) {
			position: absolute;
			top: 24px;
			left: 130px;
			height: 100px;
			width: 140px;
			background-color: var(--red);
			opacity: 1;
			clip-path: polygon(0px 0px, 140px 0px, 140px 100px, 44px 140px, 44px 36px, 0px 36px);
		}
		& > div:nth-child(4) {
			top: 176px;
			transform: scale(-1);
		}
	}
</style>

