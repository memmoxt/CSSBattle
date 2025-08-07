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
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--red: #f88889;
		--white: #ffffff;
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
			height: 300px;
			width: 400px;
			gap: 20px;
			display: grid;
			grid-template-columns: 1fr 1fr;
			grid-template-rows: 1fr 1fr;
			position: absolute;
			& > div {
				position: absolute;
				height: 140px;
				width: 190px;
				background-color: var(--red);
			}
			& > div:nth-child(2),
			& > div:nth-child(3) {
				grid-column: 2/4;
			}
			& > div:nth-child(3),
			& > div:nth-child(4) {
				grid-row: 2/4;
			}
			& > div {
				overflow: hidden;
				&:before {
					content: '';
					position: absolute;
					height: 30px;
					aspect-ratio: 1;
					translate: -4px 55px;
					border-radius: 50%;
					background-color: var(--red);
					box-shadow: 0 0 0 20px var(--white);
				}
				&:after {
					content: '';
					position: absolute;
					height: 30px;
					aspect-ratio: 1;
					translate: 164px 55px;
					border-radius: 50%;
					background-color: var(--red);
					box-shadow: 0 0 0 20px var(--white);
				}
			}
			& > div:nth-child(1) {
				&:before {
					background-color: transparent;
					box-shadow: 0 0 0 0px black;
				}
			}
			& > div:nth-child(3){
				&:after {
					background-color: transparent;
					box-shadow: 0 0 0 0px black;
				}
			}
		}
	}
</style>
