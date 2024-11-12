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
		box-sizing: border-box;
		--teal: #2f5a76;
		--yellow: #f5bb60;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1),
		& > div:nth-child(2) {
			position: absolute;
			left: 0;
			bottom: 0;
			height: 300px;
			width: 200px;
			background-color: var(--teal);
			display: flex;
			& > div {
				align-self: end;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				box-shadow:
					40px -40px 0 0 var(--yellow),
					40px -80px 0 0 var(--yellow),
					80px -120px 0 0 var(--yellow),
					120px -160px 0 0 var(--yellow),
					120px -200px 0 0 var(--yellow),
					160px -240px 0 0 var(--yellow);
			}
		}
		& > div:nth-child(2) {
			transform: translate(200px) scaleX(-1);
		}
	}
</style>

