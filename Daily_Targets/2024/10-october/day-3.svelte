<div class="main">
	<div><div></div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--purple: #594c94;
	}
	.main {
		background-color: var(--yellow);
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap-reverse;
		flex-direction: column;
		overflow: hidden;
		& > div:nth-child(1) {
			height: 80px;
			width: 260px;
			border-radius: 50%;
			transform: translateY(0px);
			overflow: hidden;
			position: absolute;
			z-index: 2;
			& > div {
				height: 80px;
				width: 260px;
				border-radius: 50%;
				background-color: var(--yellow);
				transform: translateY(-60px);
			}
		}
		& > div:nth-child(2) {
			height: 80px;
			width: 260px;
			border-radius: 50%;
			background-color: var(--purple);
			position: absolute;
			transform: translateY(-30px);
			z-index: 1;
		}
		& > div:nth-child(3) {
			height: 200px;
			width: 80px;
			transform: translateY(50px);
			background-color: var(--purple);
			z-index: 3;
		}
	}
</style>
