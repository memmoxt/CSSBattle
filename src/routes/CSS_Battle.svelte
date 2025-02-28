<div class="main">
	<div>
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
		--yellow: #ebe77e;
		--red: #de817e;
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
		column-gap: 60px;
		& > div {
			display: grid;
			height: 240px;
			width: 240px;
			grid-template-columns: repeat(3, 1fr);
			grid-template-rows: repeat(3, 1fr);
			& > div {
				height: 80px;
				width: 80px;
				background-color: var(--red);
				clip-path: polygon(0 0, 30px 0px, 30px 50px, 80px 50px, 80px 80px, 0px 80px);
			}
			& > div:nth-child(1) {
				grid-row: 1;
			}
			& > div:nth-child(2) {
				grid-row: 2;
				grid-column: 2;
			}
			& > div:nth-child(3) {
				grid-row: 3;
				grid-column: 3;
			}
		}
	}
</style>
