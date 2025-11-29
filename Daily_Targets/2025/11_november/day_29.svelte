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
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fae7df;
		--red: #be6565;
        background-color: var(--white);

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
			height: 270px;
			width: 200px;
			display: grid;
			grid-template-columns: repeat(10, 1fr);
			grid-template-rows: repeat(4, 1fr);
			row-gap: 10px;
            &>div{
                background-color:var(--red);
            }
			& > div:nth-child(1),
			div:nth-child(4),
			div:nth-child(5),
			div:nth-child(8) {
				position: relative;
				height: 60px;
				width: 100%;
			}
			& > div:nth-child(2),
			div:nth-child(3),
			div:nth-child(6),
			div:nth-child(7) {
				position: relative;
				height: 60px;
				width: 100%;
			}
			& > div:nth-child(1),
			& > div:nth-child(5) {
				grid-column: 1/4;
			}
			& > div:nth-child(2),
			& > div:nth-child(6) {
				grid-column: 5/-1;
			}
			& > div:nth-child(3),
			& > div:nth-child(7) {
				grid-column: 1/7;
			}
			& > div:nth-child(4),div:nth-child(8) {
				grid-column: 8/-1;
			}
		}
	}
</style>
