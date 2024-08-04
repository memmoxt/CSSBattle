<div class="main">
	<div>
		<div></div>
	</div>
	<div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #edaf38;
		--white: #ffffff;
		--red: #ea7457;
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
			overflow: hidden;
			height: 150px;
			aspect-ratio: 1;
			position: absolute;
			transform: translate(-75px, 75px);
			& > div {
				position: absolute;
				height: 200px;
				transform: translate(50px, 50px);
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				box-shadow: 0 0 0 50px var(--red);
			}
		}
		& > div:nth-child(2) {
			transform: translate(75px, 75px);
			& > div {
				transform: translate(-100px, 50px);
				background-color: var(--red);
				box-shadow: 0 0 0 50px var(--white);
			}
		}
	}
</style>

