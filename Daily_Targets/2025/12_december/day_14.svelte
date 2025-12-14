<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f3ac3c;
		--brown: #492d01;
		background-color: var(--yellow);
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
			height: 90px;
			translate: 90px;
			aspect-ratio: 1;
			background-color: var(--brown);
			border-radius: 50%;
			box-shadow:
				0 0 0 30px var(--yellow),
				-90px 0 var(--brown),
				-180px 0 0 30px var(--brown);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 30px;
				background-color: var(--brown);
				translate: -90px 50px;
			}
		}
	}
</style>
