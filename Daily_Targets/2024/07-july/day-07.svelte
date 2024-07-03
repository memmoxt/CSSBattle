<div class="main">
	<div class="rectangle"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--fuchsia: #be3184;
		--darkpink: #611b3f;
	}

	.main {
		height: 300px;
		width: 400px;
		background-color: var(--fuchsia);
		display: flex;
		justify-content: center;
		align-items: center;
		& > .rectangle {
			height: 80px;
			width: 160px;
			background: var(--darkpink);
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 80px;
				width: 80px;
				background-color: var(--darkpink);
				top: 150px;
				left: 40px;
				border-radius: 50px 0 0 50px;
			}
			&:after {
				transform: scaleX(-1) translate(-240px, -80px);
			}
		}
	}
</style>
