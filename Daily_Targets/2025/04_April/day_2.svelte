<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f5e3b5;
		--blue: #469dba;
        background-color:var(--yellow);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1) {
			position: absolute;
			height: 120px;
			width: 160px;
			background-color: var(--blue);
			/* opacity: 0.5; */
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--blue);
				transform: translate(140px, 40px);
				box-shadow: 0 0 0 20px var(--yellow);
			}
		}

		& > div:nth-child(2) {
			position: absolute;
			height: 80px;
			aspect-ratio: 1;
			background-color: var(--blue);
			border-radius: 50%;
			transform: translate(-80px);
			/* opacity: 0.5; */
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 150px;
				background-color: var(--blue);
				/* opacity: 0.5; */
				transform: translate(195px, 20px);
			}
		}
	}
</style>

