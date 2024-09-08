<div class="main"><div></div></div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #b5e0ba;
		--brown: #5d3a3a;
        background-color:var(--brown);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: end;
		align-items: end;
		& > div {
			height: 200px;
			aspect-ratio: 1;
			background-color: var(--green);
		}
	}
</style>

