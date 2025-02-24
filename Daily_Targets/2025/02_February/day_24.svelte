<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #343d42;
		--blue: #328fc1;
		--white: #d9d9d9;
        background-color:var(--blue);
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
			height: 240px;
			aspect-ratio: 1;
			background-color: var(--black);
			border-radius: 50%;
			transform: translateY(-10px);
			box-shadow:
				-150px 0px var(--black),
				150px 0px var(--black);
			&::before {
				content: '';
				position: absolute;
				top: 50px;
				left: 70px;
				height: 100px;
				aspect-ratio: 1;
				background-color: white;
				border-radius: 50%;
			}
			&::after {
				content: '';
				position: absolute;
				top: -20px;
				left: -100px;
				height: 50px;
				width: 450px;
				background-color: var(--black);
			}
		}
	}
</style>
