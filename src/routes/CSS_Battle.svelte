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
		box-sizing: content-box;
		--yellow: #fade8b;
		--grey: #556d7f;
		--red: #d24444;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			position: relative;
			height: 200px;
			width: 310px;
			display: grid;
			flex-wrap: wrap;
			gap: 25px 15px;
			grid-template-columns: repeat(5, 1fr);
			grid-template-rows: repeat(3, 1fr);
			& > div {
				border-radius: 50px;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--red);
			}
			& > div:nth-child(5n + 3) {
				border-radius: 0;
			}
			& > div:nth-child(5n + 2),
			div:nth-child(5n + 3),
			div:nth-child(5n + 4) {
				background-color: var(--grey);
			}
		}
	}
</style>
