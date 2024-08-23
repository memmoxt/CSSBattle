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
		--yellow: #d3b882;
		--purple: #8983ae;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
            position:absolute;
			height: 160px;
			aspect-ratio: 1;
			border-radius: 50%;
			/* border:1px solid red; */
			display: flex;
			align-items: center;
			justify-content: center;
			overflow: hidden;
			& > div {
				position: absolute;
				background-color: var(--yellow);
				height: 92px;
				aspect-ratio: 1;
				/* opacity: 0.5; */
				transform: translate(-80px) rotate(45deg);
				/* transform: translate(-80px); */
				&:before {
					position: absolute;
					content: '';
					background-color: var(--purple);
					height: 60px;
					aspect-ratio: 1;
					border-radius: 50%;
					transform: translate(16px, 16px);
				}
			}
			& > div:nth-child(2) {
				transform: translate(80px) rotate(45deg);
			}
			& > div:nth-child(3) {
				transform: translate(0px, 80px) rotate(45deg);
			}
			& > div:nth-child(4) {
				transform: translate(0px, -80px) rotate(45deg);
			}
		}
	}
</style>

