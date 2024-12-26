<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		--yellow: #fade8b;
		--purple: #594c94;
		background-color: var(--yellow);
		& > div {
			height: 240px;
			width: 320px;
			display: grid;
			grid-template-columns: repeat(7, 20px);
			grid-template-rows: 120px 60px 30px 30px;
			gap: 0px 30px;
			& > div {
				height: 100%;
				width: 100%;
				background-color: var(--purple);
			}
			& > div:nth-child(1) {
				grid-row: 4/-1;
			}
			& > div:nth-child(2) {
				grid-row: 3/-1;
			}
			& > div:nth-child(3) {
				grid-row: 2/-1;
			}
			& > div:nth-child(4) {
				grid-row: 1/-1;
			}
			& > div:nth-child(5) {
				grid-row: 2/-1;
            }
            & > div:nth-child(6) {
				grid-row: 3/-1;
			}
			& > div:nth-child(7) {
				grid-row: 4/-1;
			}
		}
	}
</style>
