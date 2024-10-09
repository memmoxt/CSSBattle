<div class="main">
	<div>
		<div>
			<div>
				<div></div>
			</div>
		</div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #b5e0ba;
		--brown: #5d3a3a;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--green);
		& > div {
			background-color: var(--brown);
			height: 200px;
			aspect-ratio: 1;
			display: flex;
			justify-content: center;
			& > div {
				height: 150px;
				aspect-ratio: 1;
				display: flex;
				background-color: var(--green);
				justify-content: right;
				align-items: center;
				& > div {
					height: 100px;
					aspect-ratio: 1;
					display: flex;
					justify-content: center;
					align-items: end;
					background-color: var(--brown);
					& > div {
						background-color: var(--green);
						height: 50px;
						aspect-ratio: 1;
					}
				}
			}
		}
	}
</style>

