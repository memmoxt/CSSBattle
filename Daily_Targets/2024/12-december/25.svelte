<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #d96c7b;
		--white: #ffffff;
        background-color:var(--red);
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
			position: absolute;
			height: 90px;
			width: 30px;
			background-color: var(--white);
			left: 75px;
			box-shadow:
				40px 0 0 var(--white),
				180px 0 0 var(--white),
				220px 0 0 var(--white);
		}
		& > div:nth-child(2) {
			transform-origin: center;
			transform: rotate(90deg);
			left: 185px;
			top: -5px;
		}
	}
</style>

