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
		--yellow: #fade8b;
		--green: #61a74e;
		--darkgreen: #3f7331;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 200px;
			aspect-ratio: 1;
			background-color: red;
			display: grid;
			grid-template-rows: repeat(2, 2fr);
			grid-template-columns: repeat(2, 2fr);
			& > div {
				height: 100px;
				aspect-ratio: 1;
				background-color: var(--green);
			}
			& > div:nth-child(4) {
				height: 0;
				border-top: 50px solid var(--darkgreen);
				border-right: 50px solid var(--yellow);
				border-bottom: 50px solid var(--yellow);
				border-left: 50px solid var(--darkgreen);
				background-color: blue;
			}
		}
	}
</style>

