<div class="main">
	<div>
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
		</div>
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
		</div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #23384b;
		--green: #00d47e;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			position: relative;
			height: 260px;
			width: 360px;
			display: flex;
			justify-content: space-around;
			gap: 100px 0px;
			flex-wrap: wrap;
			& > div {
				position: relative;
				height: 80px;
				width: 360px;
				display: grid;
				grid-template-columns: repeat(9, 1fr);
				grid-template-rows: repeat(2, 1fr);
				& > div {
					height: 40px;
					aspect-ratio: 1;
					background-color: var(--black);
					grid-row: 1;
				}
				& > div:nth-child(odd) {
					grid-row: 2;
				}
				& > div:nth-child(1) {
					grid-column: 2;
				}
				& > div:nth-child(2) {
					grid-column: 3;
				}
				& > div:nth-child(3) {
					grid-column: 4;
				}
				& > div:nth-child(4) {
					grid-column: 5;
				}
				& > div:nth-child(5) {
					grid-column: 6;
				}
				& > div:nth-child(6) {
					grid-column: 7;
				}
				& > div:nth-child(7) {
					grid-column: 8;
				}
				& > div:nth-child(8) {
					grid-column: 9;
				}
				& > div:nth-child(9) {
					grid-column: 1;
					grid-row: 1;
				}
			}
			& > div:nth-child(2) {
                background-color:var(--black);
                &>div{
                    background-color:var(--green);
                }
			}
		}
	}
</style>
