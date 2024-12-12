<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #6255aa;
		--rose: #cf81af;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color:var(--purple);
		& > div {
			position: absolute;
			top: 70px;
			left: 45px;
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--rose);
			box-shadow:
				75px 20px 0 20px var(--rose),
				209px 60px 0 60px var(--rose);
		}
	}
</style>

