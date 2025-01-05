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
		--green: #b8f4a6;
		--dark: #3ba44d;
		background-color: var(--green);
		& > div {
			height: 200px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--dark);
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 200px;
				width: 50px;
				background-color: var(--green);
				left: 175px;
			}
			&:after {
				transform: rotate(90deg);
			}
		}
	}
</style>

