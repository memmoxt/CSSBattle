<div class="main">
	<div><div></div></div>
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #222222;
		--yellow: #fade8b;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1),
		div:nth-child(2) {
			height: 120px;
			aspect-ratio: 1;
			transform: translateX(-0%);
			background-color: var(--yellow);
			overflow: hidden;
			& > div {
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				border-radius: 50%;
				transform: translate(50%, 50%);
				box-shadow: 0 0 0px 60px var(--black);
			}
		}
		& > div:nth-child(2) {
			transform: translate(0%, 0%) scale(-1, -1);
		}
	}
</style>

