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
		box-sizing: content-box;
		--yellow: #e3cc9e;
		--darkblue: #2a2753;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--yellow);

		& > div {
			position: absolute;
			display: grid;
			height: 50px;
			width: 330px;
			column-gap: 10px;
			grid-template-columns: 100px 50px 100px 50px;
			grid-template-rows: 50px;

			& > div {
				background-color: var(--darkblue);
				border-radius: 50px;
			}
		}
	}
</style>
