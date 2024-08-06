<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #49c85b;
		--white: #ffffff;
		--brown: #30230a;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1),
		div:nth-child(2) {
			position: absolute;
			border-top: 40px solid var(--brown);
			border-right: 40px solid var(--brown);
			border-bottom: 40px solid transparent;
			border-left: 40px solid transparent;
			border-radius: 50%;
		}
		& > div:nth-child(1) {
			transform: translate(-80px, -13px) rotate(-45deg);
		}
		& > div:nth-child(2) {
			transform: translate(80px, -13px) rotate(-45deg);
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 36px;
			width: 60px;
			background-color: var(--white);
			transform: translate(-150px, 132px);
			box-shadow:
				100px 0 0 var(--white),
				200px 0 0 var(--white),
				300px 0 0 var(--white);
		}
	}
</style>
