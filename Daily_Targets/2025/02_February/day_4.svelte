<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffff;
		--purple: #4b4d88;
		background-color: var(--white);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > div:nth-child(1) {
			position: absolute;
			bottom: 40px;
			height: 30px;
			width: 251px;
			border-radius: 50px/50px;
			background-color: var(--purple);
		}
		& > div:nth-child(2),
		& > div:nth-child(2):before,
		& > div:nth-child(2):after {
			position: absolute;
			content: '';
			border-radius: 50px/50px;
			height: 60px;
			width: 30px;
			background-color: var(--purple);
		}
		& > div:nth-child(2):before {
			transform: rotate(45deg);
			top: -68px;
			left: 68px;
			box-shadow: 70px 71px var(--purple);
		}
		& > div:nth-child(2):after {
			transform: rotate(-45deg);
			top: -68px;
			left: -68px;
			box-shadow: -71px 71px var(--purple);
		}
	}
</style>
