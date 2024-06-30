<div class="main">
	<div class="guide">
		<div class="big"></div>
		<div class="small"></div>
		<div class="small-2"></div>
		<div class="big-2"></div>
	</div>
</div>
<style>
	* {
		margin: 0;
		padding: 0;
		background: #998235;
	}

	.main {
		width: 100vw;
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;

		.guide {
			width: 180px;
			height: 180px;
			display: flex;
			justify-content: space-between;
			flex-wrap: wrap;
			align-content: space-between;

			.big {
				width: 80px;
				height: 100px;
				border-top-right-radius: 50px 50px;
				border-bottom-left-radius: 50px 50px;
				background-color: #1a4341;
			}

			.small {
				width: 80px;
				height: 60px;
				border-top-left-radius: 50px 50px;
				border-bottom-right-radius: 50px 50px;
				background-color: #f3ac3c;
			}

			.small-2 {
				width: 80px;
				height: 60px;
				border-top-right-radius: 50px 50px;
				border-bottom-left-radius: 50px 50px;
				transform: translate(0px, 20px);
				background-color: #f3ac3c;
			}

			.big-2 {
				width: 80px;
				height: 100px;
				border-top-left-radius: 50px 50px;
				border-bottom-right-radius: 50px 50px;
				transform: translate(0px, -20px);
				background-color: #1a4341;
			}
		}
	}
</style>
