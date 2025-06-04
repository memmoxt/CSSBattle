<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #5a9f48;
		--black: #282828;
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
		& > div:nth-child(1),
		& > div:nth-child(2) {
			position: absolute;
			background-color: var(--green);
			height: 200px;
			aspect-ratio: 1;
			border-radius: 50%;
			transform: translate(0px, -20px);
			box-shadow: 0 0 0 30px var(--black);
		}
		& > div:nth-child(2) {
			transform: translateY(-150px);
			z-index: 2;
		}
		& > div:nth-child(1) {
			clip-path: polygon(50px 50px, 150px 50px, 150px 250px, 50px 250px);
			z-index: 3;
		}
	}
</style>
