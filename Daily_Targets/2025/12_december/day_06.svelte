<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #243d83;
		--yellow: #f0cd48;
        background-color:var(--blue);
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
			height: 150px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 40px / 40px;
			border: 10px solid var(--yellow);
			overflow: hidden;
			& > div {
				height: 300px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: transparent;
				translate: -85px 75px;
				box-shadow: 0 0 0 50px var(--blue);
			}
		}
	}
</style>
