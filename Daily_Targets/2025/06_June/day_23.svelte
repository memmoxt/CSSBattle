<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #5a9f48;
		--yellow: #fade8b;
		--red: #d24444;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div,
		& > div:before {
			content: '';
			position: absolute;
			height: 160px;
			width: 120px;
			background-color: var(--yellow);
			/* opacity: 0.5; */
			border-radius: 30px/30px;
		}
		& > div:before {
			background-color: var(--yellow);
			transform: rotate(90deg);
		}
		& > div:after {
			content: '';
			position: absolute;
			height: 60px;
			aspect-ratio: 1;
			transform: translate(30px, 50px);
			border-radius: 50%;
			background-color: var(--red);
		}
	}
</style>
