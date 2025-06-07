<div class="main">
	<div class="outer"></div>
	<div class="outer"></div>
	<div class="center"></div>
	<div class="center"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #5aa4b7;
		--black: #000000;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
	}
	.center:nth-child(3),
	.center:nth-child(3):before,
	.center:nth-child(4),
	.center:nth-child(4):before {
		position: absolute;
		height: 80px;
		width: 20px;
		background-color: var(--black);
		border-radius: 20px/20px;
	}
	.center:nth-child(3):before,
	.center:nth-child(4):before {
		content: '';
		transform: rotate(-90deg);
	}

	.center:nth-child(4) {
		transform: rotate(-45deg);
	}

	.outer:nth-child(1) {
		height: 20px;
		width: 200px;
		position: absolute;
		border-radius: 50px/50px;
		background-color: var(--black);
		transform: translateY(-70px);
		box-shadow: 0 140px var(--black);
	}
	.outer:nth-child(2) {
		height: 20px;
		width: 200px;
		position: absolute;
		border-radius: 50px/50px;
		background-color: var(--black);
		transform: translateX(-70px) rotate(-90deg);
		box-shadow: 0 140px var(--black);
	}
</style>
