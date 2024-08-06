<div class="main">
	<div></div>
	<div></div>
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #49c85b;
		--white: #ffffff;
		--brown: #30230a;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1),
		& > div:nth-child(2) {
			/* opacity:0.5; */
			position: absolute;
			border-radius: 50%;
			height: 80px;
			aspect-ratio: 1;
			background-color: var(--brown);
			transform: translate(-80px, -13px);
			clip-path: polygon(-10px -100px, 100px -100px, 100px 40px, 0px 40px);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--brown);
				height: 40px;
				width: 80px;
				transform: translate(0, -49px);
			}

			&:after {
				content: '';
				position: absolute;
				background-color: var(--green);
				border-radius: 50%;
				height: 36px;
				aspect-ratio: 1;
				transform: translate(22px, 22px);
			}
		}
		& > div:nth-child(2) {
			transform: translate(80px, -13px);
			&:before {
				transform: translate(-1px, -60px) rotate(13deg);
				transform-origin: bottom right;
			}
		}
		& > div:nth-child(3) {
			height: 300px;
			width: 360px;
			display: grid;
			justify-content: center;
			align-items: end;
			grid-template-columns: repeat(4, 1fr);
			gap: 40px;
			& > div {
				height: 36px;
				width: 60px;
				background-color: var(--white);
			}
		}
	}
</style>
