<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
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
		box-sizing: content-box;
		--yellow: #f2eaa8;
		--red: #c05f6a;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		background-color: var(--red);
		& > div {
			height: 210px;
			width: 270px;
			display: grid;
			gap: 30px;
			grid-template-columns: repeat(3, 1fr);
			grid-template-rows: repeat(4, 1fr);
			& > div {
				background-color: var(--yellow);
			}
			& > div:nth-child(1),
			div:nth-child(2),
			div:nth-child(3),
			div:nth-child(3n + 2) {
			}
			& > div:nth-child(4) {
				justify-self: end;
			}
			& > div:nth-child(4),
			div:nth-child(6) {
				width: 50px;
			}
			& > div:nth-child(7) {
				justify-self: end;
			}
			& > div:nth-child(7),
			div:nth-child(9) {
				width: 30px;
			}
			& > div:nth-child(10) {
				justify-self: end;
			}
			& > div:nth-child(10),
			div:nth-child(12) {
				width: 10px;
			}
		}
	}
</style>
