<div class="main">
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f9e492;
		--black: #191919;
		--blue: #4f77ff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: grid;
		grid-template-columns: repeat(2, 100px);
		grid-template-rows: repeat(2, 100px);
		justify-content: center;
		align-content: center;
		background-color: var(--black);

		& > div {
			height: 100px;
			aspect-ratio: 1;
			overflow: hidden;
			& > div {
				height: 100px;
				aspect-ratio: 1;
				background-color: green;
				border-radius: 50%;
			}
			&:nth-child(1) > div {
				transform: translateY(50%);
				background-color: var(--yellow);
			}
			&:nth-child(2) > div {
				transform: translateX(-50%);
				background-color: var(--blue);
			}
			&:nth-child(3) > div {
				transform: translateX(50%);
				background-color: var(--blue);
			}
			&:nth-child(4) > div {
				transform: translateY(-50%);
				background-color: var(--yellow);
			}
		}
	}
</style>
