<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5aa4b7;
		--purple: #2b2a4a;
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
		& > div {
			height: 150px;
			aspect-ratio: 1;
			background-color: var(--purple);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--purple);
				border-radius: 50%;
				translate: -60px 10px;
				box-shadow:
					70px 0px var(--blue),
					150px 0 var(--blue),
					70px 80px var(--blue),
					150px 80px var(--blue),
                    220px 80px var(--purple);
			}
		}
	}
</style>
