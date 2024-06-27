<div class="main">
	<div class="big-circle"></div>
	<div class="small-circle"></div>
	<div class="retangle"></div>
</div>
<style>
	* {
		margin: 0;
		padding: 0;
		background-color: #6592cf;
	}

	.main {
		width: 100vw;
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.small-circle {
		position: absolute;
		height: 50px;
		width: 50px;
		border-radius: 50%;
		background-color: #eeb850;
	}

	.big-circle {
		position: absolute;
		height: 150px;
		aspect-ratio: 1;
		border-radius: 50%;
		border: 50px solid #6592cf;
		background-color: transparent;
	}

	.retangle {
		height: 150px;
		width: 300px;
		background-color: #243d83;
	}
</style>
