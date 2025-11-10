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
		--red: #984e77;
		--yellow: #cdc5a5;
		background-color: var(--red);
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
			height: 190px;
			width: 280px;
			display: grid;
			grid-template-columns: repeat(6, 1fr);
			grid-template-rows: repeat(3, 1fr);
			gap: 5px 20px;
			& > div {
				background-color: var(--yellow);
			}
			& > div:nth-child(7),
			& > div:nth-child(8),
			& > div:nth-child(11),
			& > div:nth-child(12) {
				background-color: transparent;
			}
			& > div:nth-child(9),
			div:nth-child(10) {
				background-color: var(--yellow);
				height: 30px;
				aspect-ratio: 1;
				border-radius: 50%;
				align-self: center;
			}
		}
	}
</style>
