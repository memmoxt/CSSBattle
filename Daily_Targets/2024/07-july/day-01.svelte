<div class="main">
	<div class="center"></div>
	<div class="arrow-right"></div>
	<div class="arrow-left"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #eff8fe;
		--blue: #4f77ff;
		background: #eff8fe;
	}

	.main {
		& > .center {
			position: absolute;
			inset: 0px 0px 0px 180Q;
			background: var(--blue);
			height: 300px;
			width: 63Q;
		}
		& > .arrow-right,
		& > .arrow-left {
			&:before {
				position: absolute;
				content: '';
				height: 64Q;
				aspect-ratio: 1;
				border-radius: 50%;
				inset: -31Q 0 0 0Q;
				background: var(--blue);
			}

			position: absolute;
			height: 165Q;
			width: 64Q;
			inset: 159Q 0 0 180Q;
			background: var(--blue);
			transform-origin: bottom;
			transform: translate(8Q, -20Q) rotate(30deg);
		}
		& > .arrow-left {
			transform: translate(-8Q, -20Q) rotate(-30deg);
		}
	}
</style>
