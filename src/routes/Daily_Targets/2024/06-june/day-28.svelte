<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--light-blue: #6592cf;
		--blue: #243d83;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: start;
		align-items: center;
		background-color: var(--light-blue);
		& > div:nth-child(1) {
			height: 90px;
			width: 280px;
			background-color: var(--blue);
		}
		& > div:nth-child(2) {
			height: 60px;
			width: 280px;
			background-color: var(--light-blue);
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--light-blue);
				transform: translate(110px, 100%);
			}
		}
		& > div:nth-child(3) {
			height: 150px;
			width: 280px;
			background-color: var(--blue);
		}
	}
</style>
