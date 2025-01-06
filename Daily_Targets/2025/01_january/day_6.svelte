<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		--light: #b8dcf0;
		--dark: #3f4869;
        background-color:var(--light);
		& > div {
			height: 70px;
			aspect-ratio: 1;
			background-color: var(--dark);
			box-shadow:
				-120px 120px 0 50px var(--dark),
				120px -120px 0 50px var(--dark);
			transform: rotate(-45deg);
		}
	}
</style>

