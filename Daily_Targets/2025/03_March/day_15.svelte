<div class="main">
	<div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #4f77ff;
		--white: #ffffff;
        background-color:var(--blue)
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
		& > div {
			height: 128px;
			aspect-ratio: 1;
			background-color: var(--blue);
			/* background-color: red; */
			/* opacity: 0.5; */
			border-radius: 50%;
			box-shadow: 0 0 0 32px var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 32px;
				width: 256px;
				background-color: var(--white);
				/* background-color: green; */
				transform: translate(-64px, 128px);
			}
		}
	}
</style>

