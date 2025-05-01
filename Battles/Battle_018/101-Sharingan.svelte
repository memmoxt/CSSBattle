<div class="main">
	<div class="main-ball">
		<div class="circles"></div>
		<div class="center"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--brown: #161616;
		--black: #000000;
		--red: #a22015;
		--orange: #e96a23;
        background-color: var(--brown);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
	}
	.main-ball {
		position: absolute;
		height: 190px;
		aspect-ratio: 1;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color:var(--red);
		border-radius: 50%;
		box-shadow: 0 0 0 5px var(--black);
        overflow:hidden;
	}
	.circles {
		position: absolute;
		height: 70px;
		aspect-ratio: 1;
		background-color: var(--red);
		border-radius: 50%;
		box-shadow:
			74px -42px var(--red),
			-74px -42px var(--red),
			0 85px var(--red),
			0 0 0 15px var(--black),
			0 85px 0 15px var(--black),
			74px -42px 0 15px var(--black),
			-74px -42px 0 15px var(--black);
	}
	.center {
		position: absolute;
		height: 50px;
		aspect-ratio: 1;
		background-color: var(--black);
		border-radius: 50%;
		box-shadow: 0 0 0 10px var(--orange);
	}
</style>
