<div class="main">
	<div class="grid_center">
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
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		--green: #0b2429;
		--yellow: #f3ac3c;
        background-color:var(--green);
		& > .grid_center {
			height: 156px;
			width: 300px;
			display: grid;
			row-gap: 15px;
			grid-template-columns: 100px 100px 100px;
			grid-template-rows: 70px 70px;
			& > div {
				justify-self: center;
				background-color: var(--yellow);
			}
			& > div:nth-child(odd) {
				height: 70px;
				width: 70px;
			}
			& > div:nth-child(even) {
				width: 100px;
				height: 70px;
			}
		}
	}
</style>

