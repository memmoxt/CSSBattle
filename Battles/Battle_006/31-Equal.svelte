<div class="main">
	<div class="yellow"></div>
	<div class="orange"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		background: #aa445f;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;

		& > .yellow {
			height: 200px;
			width: 100px;
			overflow: hidden;
			transform: translate(-25%, 0);

			&:before {
				content: '';
				position: absolute;
				height: 200px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: #f7ec7d;
			}
		}

		& > .orange {
			height: 200px;
			width: 100px;
			overflow: hidden;
			transform: translate(25%, 0);

			&:before {
				content: '';
				position: absolute;
				height: 200px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(-50%, 0);
				background-color: #e38f66;
			}
		}
	}
</style>
