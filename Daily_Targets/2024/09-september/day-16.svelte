<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #ea333d;
		--black: #191919;
		--white: #ffffff;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 140px;
			width: 200px;
			background-color: var(--red);
			border-radius: 40px;
			display: flex;
			justify-content: center;
			align-items: center;
			& > div {
				transform: translateX(8px);
				border-top: 30px solid var(--red);
				border-right: 0px solid var(--red);
				border-bottom: 30px solid var(--red);
				border-left: 50.0px solid var(--white);
			}
		}
	}
</style>

