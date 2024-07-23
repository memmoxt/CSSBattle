<div class="main">
	<div class="center">
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
		--red: #b53733;
		--orange: #ea7457;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background: var(--red);
		& > .center {
			height: 300px;
			width: 400px;
			display: grid;
			justify-content: center;
			align-items: center;
			grid-template-columns: repeat(9, 20px);
			grid-template-rows: repeat(1, 300px);
			gap: 20px;
			& > div {
				height: 150px;
				width: 20px;
				background-color: var(--orange);
			}
			& > div:nth-child(1),
			div:nth-child(9) {
				height: 140px;
				align-self: start;
			}
			& > div:nth-child(2),
			div:nth-last-child(2) {
				transform: translateY(-45px);
			}
			& > div:nth-child(3),
			div:nth-last-child(3) {
				transform: translateY(-5px);
			}
			& > div:nth-child(4),
			div:nth-last-child(4) {
				transform: translateY(35px);
			}
			& > div:nth-child(5) {
				align-self: end;
			}
		}
	}
</style>
