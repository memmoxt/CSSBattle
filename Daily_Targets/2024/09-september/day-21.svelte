<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fae29e;
		--green: #4a9a86;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
		grid-template-columns: 150px 100px 150px;
		grid-template-rows: repeat(6, 50px);
		& > div {
			height: 50px;
			aspect-ratio: 1;
			grid-column: 2;
            background-color: var(--yellow);
		}
		& > div:nth-child(odd) {
            justify-self:end;
		}
	}
</style>

