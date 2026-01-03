<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #84b9c7;
		--white: #ecebeb;
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
			position: absolute;
			height: 200px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				background-color: var(--blue);
				translate: 50px -50px;
				border-radius: 50%;
				box-shadow:
					0px 200px var(--blue),
					-100px 100px var(--white),
					100px 100px var(--white);
			}
		}
	}
</style>
