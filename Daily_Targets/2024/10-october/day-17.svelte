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
		--orange: #e38f66;
		--white: #f7f3d7;
        background-color:var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 140px;
			width: 320px;
			display: grid;
			grid-template-rows: repeat(3, 1fr);
			grid-template-columns: repeat(3, 1fr);
			gap: 8px;
			& > div {
				background-color: var(--white);
			}
		}
	}
</style>

