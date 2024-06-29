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
				display: flex;
				justify-content: space-around;
			}
			& > .second-row {
				display: flex;
				justify-content: space-around;
				margin: -20px -40px;
			}
		}
	}
</style>
