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
		--green: #8ab8b6;
		--red: #d96c7b;
		--white: #f3ead2;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
		grid-template-columns: repeat(6, 60px);
		grid-template-rows: 1fr 60px 1fr;
		& > div {
			height: 60px;
			background-color: var(--red);
			grid-row: 2;
            border-radius:50%;
		}
		& > div:nth-child(odd) {
			border-top-right-radius: 0%;
            border-bottom-right-radius:0%;
            background-color:var(--white);

		}
	}
</style>

