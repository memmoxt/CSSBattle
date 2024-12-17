<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #588a95;
		--white: #ffffff;
        background-color:var(--green);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			height: 180px;
			aspect-ratio: 1;
			position: absolute;
			overflow: hidden;
			& > div {
				position: absolute;
				height: 12px;
				aspect-ratio: 1;
				background-color: var(--green);
				right: 0px;
				bottom: 0px;
				box-shadow:
					0 0 0 24px var(--white),
					0 0 0 48px var(--green),
					0 0 0 72px var(--white),
					0 0 0 96px var(--green),
					0 0 0 120px var(--white),
					0 0 0 144px var(--green),
					0 0 0 168px var(--white);
			}
		}
	}
</style>

