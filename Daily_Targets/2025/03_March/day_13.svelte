<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #ffe8bd;
		--blue: #31798f;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		background-color: var(--yellow);
		& > div:nth-child(1) {
			position: absolute;
			height: 65px;
			width: 240px;
			background-color: transparent;
			transform: translate(0, -73px);
			overflow: hidden;
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				border-radius: 50%;
				transform: translate(40px, 40px);
				box-shadow: 0 0 0 40px var(--blue);
			}
			&:after {
				transform: translate(140px, 40px);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 145px;
			background-color: var(--blue);
			transform: translate(0px, 32px);
			width: 40px;
			box-shadow:
				-100px 0 0 var(--blue),
				100px 0 0 var(--blue);
		}
	}
</style>

