<div class="main">
	<div>
		<div>
			<div>
				<div><div><div></div></div></div>
			</div>
		</div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--red: #e3516e;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--red);
		& > div {
			overflow: hidden;
			position: absolute;
			height: 160px;
			width: 120px;
			border-radius: 60px/60px;
			background-color: var(--yellow);
			& > div {
				border-radius: 50%;
				height: 140px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				box-shadow: 0 0 0px 10px var(--red);
				transform: translate(0px, 20px);
				& > div {
					border-radius: 50%;
					height: 120px;
					width: 120px;
					background-color: var(--yellow);
					box-shadow: 0 0 0px 10px var(--red);
					transform: translate(20px, 25px);
					& > div {
						border-radius: 50%;
						height: 100px;
						aspect-ratio: 1;
						background-color: var(--yellow);
						box-shadow: 0 0 0px 10px var(--red);
						transform: translate(20px, 25px);
						& > div {
							border-radius: 50%;
							height: 80px;
							aspect-ratio: 1;
							background-color: var(--yellow);
							box-shadow: 0 0 0px 10px var(--red);
							transform: translate(20px, 25px);
							& > div {
								border-radius: 50%;
								height: 60px;
								aspect-ratio: 1;
								background-color: var(--yellow);
								box-shadow: 0 0 0px 10px var(--red);
								transform: translate(20px, 25px);
							}
						}
					}
				}
			}
		}
	}
</style>
