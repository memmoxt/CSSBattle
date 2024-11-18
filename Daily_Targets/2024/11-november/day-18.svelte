<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--teal: #2f5a76;
		--yellow: #f5bb60;
		background-color: var(--teal);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 200px;
			width: 120px;
			overflow: hidden;
			& > div {
				position: absolute;
				top: 52px;
				left: -28px;
				height: 175px;
				aspect-ratio: 1;
				background-color: transparent;
				box-shadow: 0 0 0 40px var(--yellow);
				border-radius: 50%;
				&:before {
					content: '';
					position: absolute;
					height: 140px;
					width: 40px;
					background-color: var(--yellow);
					top: -5px;
					left: 68px;
				}
			}
		}
	}
</style>
