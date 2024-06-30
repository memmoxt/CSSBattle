<div class="main">
	<div class="center">
		<div class="first-row">
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="second-row">
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #feff58;
		--orange: #f48b26;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--orange);
		overflow: hidden;
		& > .center {
			height: 120px;
			width: 400px;
			& > div > div {
				height: 70px;
				width: 60px;
				background-color: var(--yellow);
			}
			& > .first-row {
				/* border:1px solid blue; */
				height: 70px;
				margin-bottom: -20px;
				display: grid;
				grid-template-columns: repeat(5, auto);
				justify-content: space-around;
			}
			& > .second-row {
				height: 70px;
				display: grid;
				justify-content: space-around;
				gap: 20px;
				grid-template-columns: repeat(6, 60px);
			}
		}
	}
</style>
