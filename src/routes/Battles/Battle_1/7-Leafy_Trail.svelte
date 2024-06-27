<div class="main">
	<div class="first"></div>
	<div class="middle"></div>
	<div class="end"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		background-color: #0b2429;
	}

	.main {
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.first {
		position: absolute;
		border-top-left-radius: calc(100% / 3 * 2);
		border-bottom-right-radius: calc(100% / 3 * 2);
		width: 150px;
		aspect-ratio: 1;
		background-color: #998235;
		z-index: 1;
	}

	.middle {
		position: absolute;
		border-top-left-radius: calc(100% / 3 * 2);
		border-bottom-right-radius: calc(100% / 3 * 2);
		transform: translate(calc(100% / 3 * -1), 0%);
		width: 150px;
		height: 150px;
		background-color: #1a4341;
		z-index: 0;
	}

	.end {
		position: absolute;
		border-top-left-radius: calc(100% / 3 * 2);
		border-bottom-right-radius: calc(100% / 3 * 2);
		transform: translate(calc(100% / 3), 0%);
		width: 150px;
		height: 150px;
		background-color: #f3ac3c;
		z-index: 2;
	}
</style>
