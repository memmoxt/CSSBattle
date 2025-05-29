<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--orange: #f58220;
		--black: #282828;
		--white: #ffffff;
        background-color:var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;

		& > div {
			height: 80px;
			aspect-ratio: 1;
			background-color: var(--black);
			border-radius: 50%;
			box-shadow:
				-200px -80px 0 20px var(--white),
				-200px 80px 0 20px var(--black),
				200px -80px 0 20px var(--black),
				200px 80px 0 20px var(--white);
		}
	}
</style>
