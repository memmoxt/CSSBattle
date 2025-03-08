<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffeff7;
		--blue: #226aa9;
		--yellow: #deb467;
		--black: #000000;
        background-color:var(--white);
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
		& > div:nth-child(1) {
			position: absolute;
			height: 160px;
			width: 170px;
			background-color: var(--blue);
			transform: translate(-140px);
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 160px;
			width: 110px;
			background-color: var(--yellow);
			transform: translate(0px);
            clip-path: polygon(0 0, 100% 50%, 0 100%);
			&:before {
				position: absolute;
				content: '';
				background-color: var(--black);
				height: 100px;
				transform: translate(60px, 30px);
				aspect-ratio: 1;
				border-radius: 50%;
			}
		}
	}
</style>

