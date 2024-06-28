<div class="main">
	<div class="big-box">
		<div class="medium-box">
			<div class="small-box"></div>
		</div>
	</div>
</div>
<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		background: #f3ac3c;
	}

	.main {
		width: 100vw;
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;

		.big-box {
			height: 200px;
			aspect-ratio: 1;
			background-color: #1a4341;
			display: flex;

			.medium-box {
				height: 100px;
				aspect-ratio: 1;
				background-color: #998235;
				align-self: end;
				display: flex;
				justify-content: end;

				.small-box {
					height: 50px;
					aspect-ratio: 1;
					background-color: #f3ac3c;
					align-self: end;
				}
			}
		}
	}
</style>
