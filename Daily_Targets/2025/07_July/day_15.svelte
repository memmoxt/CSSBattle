<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #2f5a76;
		--yellow: #f5bb60;
		background-color: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 30px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 50%;
			translate: -160px 0px;
			box-shadow:
				130px 0 var(--yellow),
				260px 0 var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 270px;
				translate: 110px -135px;
				background-color: var(--yellow);
				box-shadow: 0px 270px var(--yellow);
			}
		}
	}
</style>
