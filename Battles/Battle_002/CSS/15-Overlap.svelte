<div class="main">
	<div class="circle"></div>
	<div class="circle other"></div>
</div>
<style>
	* {
		background: #09042a;
		margin: 0;
	}

	.main {
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.circle {
		width: 150px;
		aspect-ratio: 1;
		border-radius: 50%;
		margin: -25px;
		background: #7b3f61;
	}

	.other {
		background-color: #e78481;
		position: relative;
		overflow: hidden;

		&:before {
			content: '';
			position: absolute;
			width: 150px;
			aspect-ratio: 1;
			background-color: #09042a;
			border-radius: 50%;
			transform: translate(calc(-100% * 2 / 3), 0%);
		}
	}
</style>
