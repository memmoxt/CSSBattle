<div class="main">
	<div>
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
		--stone: #f4dcbf;
		--slate: #556d7f;
		--brown: #3c342a;
		background-color: var(--stone);
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
			height: 80px;
			width: 200px;
			display: grid;
			grid-template-columns: 60px 60px 60px;
			grid-template-rows: repeat(2, 1fr);
			justify-content: center;
			align-items: center;
			background-color: var(--slate);
			& > div {
				height: 20px;
				width: 40px;
				place-self: center;
				background-color: var(--stone);
			}
			& > div:nth-child(1),
			div:nth-child(3),
			div:nth-child(4),
			div:nth-child(6) {
				background-color: var(--brown);
			}
		}
	}
</style>
