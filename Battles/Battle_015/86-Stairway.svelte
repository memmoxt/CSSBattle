<div class="main"> 
	<div>
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
		--black: #191919;
		--blue: #4f77ff;
		background-color: var(--black);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;

		& > div {
			height: 150px;
			width: 100px;
			background-color: var(--blue);
			/* opacity: 0.5; */
			border-top-right-radius: 50px;
			border-top-left-radius: 50px;
			display: grid;
			row-gap: 4px;
			grid-template-rows: 55px repeat(4, 1fr);
			grid-template-columns: repeat(5, 4fr);

			& > div {
				background-color: var(--black);
			}
			& > div:nth-child(1) {
				grid-column: 2/6;
				grid-row: 5;
			}
			& > div:nth-child(2) {
				grid-column: 3/6;
				grid-row: 4;
			}
			& > div:nth-child(3) {
				grid-column: 4/6;
				grid-row: 3;
			}
			& > div:nth-child(4) {
				grid-column: 5/6;
				grid-row: 2;
			}
		}
	}
</style>
