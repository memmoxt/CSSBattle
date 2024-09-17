<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fcebeb;
		--orange: #ea9a52;
		--blue: #515697;
		background-color: var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 100px;
			width: 400px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				transform: translate(150%, -100%);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				transform: translate(150%, 100%);
				background-color: var(--blue);
			}
		}
	}
</style>
