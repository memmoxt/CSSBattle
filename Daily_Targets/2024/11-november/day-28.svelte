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
		--green: #2f5a76;
		--yellow: #f5bb60;
		--red: #f56760;
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
			overflow: hidden;
			position: absolute;
			height: 220px;
            background-color:var(--green);
			aspect-ratio: 1;
			& > div {
				position: absolute;
				height: 220px;
				aspect-ratio: 1;
				background-color: var(--red);
				border-radius: 50%;
				clip-path: polygon(110px 0px, 220px 0px, 220px 110px, 110px 110px);
				transform: translate(110px) rotate(-90deg);
			}
			& > div:nth-child(2) {
				background-color: var(--red);
				transform: translate(-110px) rotate(90deg);
			}
			& > div:nth-child(3) {
				background-color: var(--yellow);
				transform: translateY(-110px) rotate(180deg);
			}
			& > div:nth-child(4) {
				background-color: var(--yellow);
				transform: translateY(110px) rotate(0deg);
			}
		}
	}
</style>

