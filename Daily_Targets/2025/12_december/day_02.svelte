<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--beige: #696448;
		--black: #222222;
		--white: #ffffff;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		background-color: var(--beige);
		& > div:nth-child(1) {
			position: absolute;
			height: 100px;
			width: 50px;
			background-color: var(--white);
		}
		& > div:nth-child(2),
		div:nth-child(3) {
			position: absolute;
			height: 140px;
			aspect-ratio: 1;
			translate: -30px;
			border-radius: 50%;
			border: 30px solid var(--black);
			background-color: transparent;
		}
		& > div:nth-child(3) {
			translate: 30px;
		}
	}
</style>
