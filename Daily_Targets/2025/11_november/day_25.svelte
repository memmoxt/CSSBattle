<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--light: #aadbf7;
		--blue: #328fc1;
		--dark: #243d83;
        background-color: var(--light);
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
			height: 110px;
			aspect-ratio: 1;
			background-color: var(--blue);
			box-shadow: 0 0 0 20px var(--dark);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--blue);
				translate: -70px 80px;
				box-shadow:
					0 0 0 20px var(--dark),
					220px 0 var(--blue),
					220px 0 0 20px var(--dark);
			}
		}
	}
</style>
