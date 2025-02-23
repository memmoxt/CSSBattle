<div class="main">
	<div>
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
		box-sizing: content-box;
		--yellow: #eac049;
		--blue: #51a499;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 300px;
			width: 180px;
			display: grid;
			grid-template-columns: 1fr;
			grid-template-rows: repeat(12, 1fr);
			& > div {
				background-color: var(--blue);
			}
			& > div:nth-child(1) {
				grid-row-start: 9;
			}
			& > div:nth-child(2) {
				grid-row-start: 11;
				grid-row-end: span 2;
			}
			& > div:nth-child(3) {
				grid-row-start: 6;
				grid-row-end: span 2;
			}
			& > div:nth-child(4) {
				grid-row-start: 4;
			}
			& > div:nth-child(5) {
				grid-row-start: 1;
				grid-row-end: span 2;
			}
		}
	}
</style>

