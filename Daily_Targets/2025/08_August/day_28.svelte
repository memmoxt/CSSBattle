<div class="main">
	<div class="left"></div>
	<div class="right"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #b6ebe7;
		--purple: #724faf;
		background-color: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
	}
	.left {
		content: '';
		position: absolute;
		height: 50px;
		aspect-ratio: 1;
		background-color: var(--purple);
		translate: -100px -40px;
		&:before {
			content: '';
			position: absolute;
			height: 70px;
			width: 10px;
			background-color: var(--purple);
			translate: 20px 50px;
		}
		&:after {
			content: '';
			position: absolute;
			height: 10px;
			width: 50px;
			background-color: var(--purple);
			translate: 20px 60px;
			box-shadow: 0px 50px var(--purple);
		}
	}
	.right {
		content: '';
		position: absolute;
		height: 30px;
		width: 110px;
		background-color: var(--purple);
		box-shadow:
			0px -50px var(--purple),
			0px 50px var(--purple);
	}
</style>
