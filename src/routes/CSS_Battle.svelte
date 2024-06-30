<div class="main">
	<div class="center"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--dark:#191919;
        --yellow:#F2AD43;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > .center {
			height: 100px;
			width: 250px;
			background-color: var(--yellow);
            opacity:0.5;
            box-shadow: 0 0 0;
		}
	}
</style>
