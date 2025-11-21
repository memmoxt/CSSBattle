<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #c899e8;
		--dark: #a455d9;
        background-color:var(--dark);
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
			height: 120px;
			width: 100px;
			background-color: var(--purple);
			border-radius: 50px/50px;
			box-shadow:
				0px 140px var(--purple),
				0 -140px var(--purple),
				120px 70px var(--purple),
				120px -70px var(--purple),
				-120px -70px var(--purple),
				-120px 70px var(--purple);
		}
	}
</style>
