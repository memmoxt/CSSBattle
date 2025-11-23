<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #51a499;
		--yellow: #eded87;
		--black: #000000;
		background-color: var(--green);
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
			width: 20px;
			background-color: var(--yellow);
			box-shadow:
				20px -10px var(--black),
				20px 10px var(--black),
				40px 20px var(--yellow),
				40px -20px var(--yellow),
				60px 30px var(--black),
				60px -30px var(--black),
				200px 30px var(--black),
				200px -30px var(--black),
				220px 20px var(--yellow),
				220px -20px var(--yellow),
				240px 10px var(--black),
				240px -10px var(--black),
				260px 0px var(--yellow);
			translate: -130px;
			&:before {
				content: '';
				position: absolute;
				height: 180px;
				width: 120px;
				background-color: var(--yellow);
				translate: 80px -45px;
			}
		}
	}
</style>
