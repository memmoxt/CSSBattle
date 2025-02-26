<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #46ba67;
		--purple: #4c4c6b;
		--yellow: #fae29e;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		column-gap: 60px;
		grid-template-rows: 1fr 40px 1fr;
		grid-template-columns: repeat(3, 40px);
		& > div {
			height: 130px;
			width: 40px;
			background-color: red;
			/* opacity: 0.5; */
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: black;
				border-radius: 50%;
				transform: translateY(130px);
			}
		}
		& > div:nth-child(1) {
			grid-row: -2;
			transform: scaleY(-1);
			background-color: var(--purple);
			&:before {
				background-color: var(--yellow);
			}
		}
		& > div:nth-child(2) {
			grid-column: 2;
			background-color: var(--yellow);
			&:before {
				background-color: var(--purple);
			}
		}
		& > div:nth-child(3) {
			grid-row: -2;
			grid-column: -2;
			transform: scaleY(-1);
			background-color: var(--purple);
			&:before {
				background-color: var(--yellow);
			}
		}
	}
</style>

