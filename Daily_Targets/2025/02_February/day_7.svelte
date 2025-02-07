<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--amber: #ea9a52;
		--dark: #96551a;
        background-color:var(--amber);
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
		& > div:nth-child(2),
		& > div:nth-child(3) {
			height: 160px;
			aspect-ratio: 1;
			background-color: var(--amber);
			border-radius: 50%;
			box-shadow: 0 0 0 40px var(--dark);
			clip-path: polygon(-40px 70px, 200px 70px, 200px 200px, -40px 200px);
		}
		& > div:nth-child(1) {
			transform: translate(60px, 0px) rotate(180deg);
		}
		& > div:nth-child(3) {
			transform: translate(-60px, 0px) rotate(180deg);
		}
		& > div:nth-child(4) {
			position: absolute;
			height: 20px;
			width: 400px;
            background-color:var(--dark);
		}
	}
</style>

