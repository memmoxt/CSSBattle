<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #d86f45;
		--yellow: #fade8b;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--yellow);
		& > div {
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--orange);
		}
		&:before {
			content: '';
			position: absolute;
			height: 100px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--yellow);
			transform: translate(-50%, -50%);
			opacity: 100%;
			box-shadow:
				100px 0 0 0 var(--yellow),
				0px 100px 0 0 var(--yellow),
				100px 100px 0 0 var(--yellow);
		}
		&:after {
			content: '';
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--orange);
			opacity: 100%;
			border-radius: 50%;
			transform: translate(-50px, -50px);
			box-shadow: 100px 100px 0 0 var(--orange);
		}
	}
</style>
