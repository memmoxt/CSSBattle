<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
        position:absolute;
		--red: #d94e4e;
		--black: #010201;
		--yellow: #feff58;
		background-color: var(--red);
		& > div:nth-child(1) {
			height: 200px;
			width: 100px;
			background-color: var(--black);
			translate: 0 50px;
			position: absolute;
			&:before {
				content: '';
				position: absolute;
				height: 70px;
				width: 30px;
				background-color: var(--black);
				translate: -105px 60px;
				box-shadow: 280px 0px var(--black);
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				width: 300px;
				background-color: var(--black);
				translate: -100px 100px;
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 190px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--red);
			translate: 0 -150px;
			box-shadow: 0 0 0 30px var(--yellow);
		}
	}
</style>
