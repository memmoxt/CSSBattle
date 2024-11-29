<div class="main">
	<div>
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
		overflow: hidden;
		position: absolute;
		--brown: #35312f;
		--yellow: #f3ac3c;
        background-color:var(--brown);
		& > div {
			position: absolute;
			overflow: hidden;
			height: 220px;
			background-color: var(--brown);
			aspect-ratio: 1;
			display: flex;
			justify-content: center;
			align-items: center;
			&:before {
				position: absolute;
				content: '';
				height: 200px;
				aspect-ratio: 1;
				background-color: var(--yellow);
			}

			& > div {
				position: absolute;
				height: 56px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				box-shadow: 0 0 0 16px var(--brown);
			}
			& > div:nth-child(1) {
				transform: translate(-72px, -72px);
			}
			& > div:nth-child(2) {
				transform: translate(-72px, 72px);
			}
			& > div:nth-child(3) {
				transform: translate(72px, 72px);
			}
			& > div:nth-child(4) {
				transform: translate(72px, -72px);
			}
		}
	}
</style>

