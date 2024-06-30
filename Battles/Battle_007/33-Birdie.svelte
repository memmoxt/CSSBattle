<div class="main">
	<div class="half-circle"></div>
	<div class="quarter"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		background: #1a4341;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		transform: translate(12px, 0px);

		.half-circle {
			height: 150px;
			aspect-ratio: 1/2;
			transform: translate(0px, 0px);
			overflow: hidden;
			background-color: transparent;

			&:before {
				content: '';
				position: absolute;
				height: 150px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: #998235;
			}

			&:after {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(30px, 30px);
				background-color: #0b2429;
			}
		}

		.quarter {
			height: 100px;
			aspect-ratio: 1;
			background-color: transform;
			overflow: hidden;
			transform: translate(0%, -50%);

			&:before {
				content: '';
				position: absolute;
				height: 200px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: #f3ac3c;
				transform: translate(-50%, 0%);
			}
		}
	}
</style>
