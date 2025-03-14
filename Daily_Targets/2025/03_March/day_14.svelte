<div class="main">
	<div>
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
		--pink: #d96c7b;
		--rose: #8b0051;
		background-color: var(--pink);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 75px;
			width: 240px;
			background-color: transparent;
			transform: translate(0, 69px);
			display: grid;
			grid-template-columns: repeat(3, 1fr);
			grid-template-rows: 1fr;
			column-gap: 60px;
			& > div {
				width: 40px;
				height: 74px;
				background-color: var(--rose);
			}
		}
	}
</style>

