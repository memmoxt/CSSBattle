<div class="main">
	<div class="semi first"></div>
	<div class="semi middle"></div>
	<div class="semi end"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		background-color: #f5d6b4;
	}

	.main {
		display: flex;
		height: 100vh;
		width: 100vw;
		justify-content: center;
		align-items: center;
	}

	.semi {
		height: calc(100vh / 5);
		aspect-ratio: 1;
		border-radius: 50%;
		background-color: transparent;
		border-top: 20px solid #d86f45;
		border-right: 20px solid #d86f45;
		border-bottom: 20px solid transparent;
		border-left: 20px solid transparent;

		&::before {
			content: '';
			position: absolute;
			height: 20px;
			transform: translate(-8px, -8px);
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: #d86f45;
		}
	}

	.first {
		transform: scaleX(-1) rotate(135deg);
	}

	.middle {
		transform: rotate(-45deg);
		margin: -20px;
	}

	.end {
		transform: rotate(135deg);
	}
</style>
