<div class="main">
	<div class="first"></div>
	<div class="second"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #2d3464;
		--yellow: #dab897;
        background-color:var(--blue);
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
	}
	.first {
		/* opacity: 0.5; */
		position: absolute;
		transform: translate(0, 40px);
		height: 141px;
		width: 30px;
		background-color: var(--blue);
        z-index:2;
	}
	.first:before {
		content: '';
		position: absolute;
		height: 60px;
		width: 30px;
		background-color: var(--yellow);
	}
	.second {
		--ball: 201px;
		position: absolute;
		height: var(--ball);
		aspect-ratio: 1;
		background-color: var(--yellow);
		/* opacity: 0.5; */
		border-radius: 50%;
		bottom: calc(0px - (var(--ball)) / 2);
		/* overflow:hidden; */
        z-index:1;
		&:before {
			content: '';
			position: absolute;
			height: 40px;
			width: 70px;
			background-color: var(--blue);
			transform: translate(-20px, 70px);
            box-shadow: 170px 0 0 var(--blue);
		}
	}
</style>

