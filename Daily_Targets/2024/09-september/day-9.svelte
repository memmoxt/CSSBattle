<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fcebeb;
		--red: #e95d29;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 150px;
			aspect-ratio: 1;
			background-color: var(--red);
			border-radius: 50%;
			transform: translate(-37%, -25%);
			position: absolute;
		}

		& > div:nth-child(2) {
			transform: translate(36%, -25%);
			&:before {
				content: '';
				position: absolute;
				background: var(--red);
				height: 150px;
				aspect-ratio: 1;
				transform-origin: bottom left;
				transform: translate(21px, 86px) rotate(-45deg);
			}
		}
	}
</style>

