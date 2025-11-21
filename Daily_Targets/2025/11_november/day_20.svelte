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
		box-sizing: border-box;
		--white: #eed9d9;
		--green: #668884;
		--orange: #c67455;
        background-color:var(--white);
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
			position: absolute;
			height: 150px;
			width: 150px;
			display: grid;
			grid-template-rows: repeat(3, 1fr);
			grid-template-columns: repeat(3, 1fr);
			& > div {
				height: 100%;
				width: 100%;
				border-top-left-radius: 50px;
				border-bottom-left-radius: 50px;
			}
			& > div:nth-child(1),
			div:nth-child(4) {
                background-color:var(--green);
				grid-column: 2/3;
			}
			& > div:nth-child(4) {
				grid-row: -1/-2;
			}
			& > div:nth-child(2),
			div:nth-child(3) {
                background-color: var(--orange);
				grid-row: 2/3;
			}
			& > div:nth-child(3) {
				grid-column: 3/4;
				transform: rotate(180deg);
			}
		}
	}
</style>
