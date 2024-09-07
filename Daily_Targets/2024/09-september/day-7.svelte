<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #de817e;
		--green: #217e81;
		background-color: var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 142px;
			aspect-ratio: 1;
			background-color: var(--green);
			/* opacity: 50%; */
			transform: rotate(45deg);
			display: flex;
			align-items: center;
			justify-content: center;
			& > div {
				height: 58px;
				aspect-ratio: 1;
				background-color: var(--red);
				box-shadow:
					58px 58px 0px var(--red),
					-58px -58px 0px var(--red);
			}
		}
	}
</style>
