<div class="main">
	<div class="guide">
		<div class="semi-circle"></div>
		<div class="semi-circle"></div>
		<div class="semi-circle rt"></div>
	</div>
</div>
<style>
	* {
		margin: 0;
		padding: 0;
		background: #6592cf;
	}

	.main {
		width: 100vw;
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;

		.guide {
			width: 320px;
			height: 220px;
			display: grid;
			grid-template-columns: 80px 40px 80px;
			grid-template-rows: 40px 60px 40px;

			:nth-child(1) {
				grid-column: 1/2;
			}

			:nth-child(2) {
				grid-column: -1;
			}

			:nth-child(3) {
				grid-row: 3;
				grid-column: 3;
			}

			.semi-circle {
				height: 80px;
				aspect-ratio: 1;
				border-radius: 50%;
				border-top: 20px solid #060f55;
				border-bottom: 20px solid #6592cf;
				border-left: 20px solid #6592cf;
				border-right: 20px solid #060f55;
				background-color: transparent;
				transform: rotate(-45deg);
			}

			.rt {
				transform: rotate(135deg) translate(14px, 14px);
			}
		}
	}
</style>
