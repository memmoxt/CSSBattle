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
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--blue: #587795;
		--yellow: #e8ad6d;
        background-color:var(--blue);
		& > div {
			display: grid;
			height: 160px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			padding: 10px;
			gap: 40px;
			grid-template-columns: repeat(3, 1fr);
			grid-template-rows: repeat(3, 1fr);
			& > div {
				border-radius: 50%;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--blue);
			}
		}
	}
</style>

