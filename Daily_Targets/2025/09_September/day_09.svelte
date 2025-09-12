<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #00b1d4;
		--black: #142032;
		background-color: var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1),
		& > div:nth-child(1):before,
		& > div:nth-child(1):after {
			position: absolute;
			content: '';
			height: 20px;
			aspect-ratio: 1;
			background-color: var(--blue);
			translate: -80px -80px;
			box-shadow:
				0 0 0 10px var(--black),
				0 0 0 20px var(--blue);
		}
		& > div:nth-child(1):before {
			translate: 160px;
		}
		& > div:nth-child(1):after {
			translate: 0px 160px;
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 160px;
			aspect-ratio: 1;
			background-color: var(--black);
			box-shadow: 0px 0px 0 30px var(--blue);
			clip-path: polygon(80px 80px, 190px 80px, 190px 190px, 80px 190px);
		}
	}
</style>
