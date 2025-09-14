<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fffbda;
		--black: #30383f;
		--red: #d96c7b;
        background-color: var(--white);
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
			--ball: var(--black);
			--background: var(--red);
			position: absolute;
			height: 60px;
			width: 360px;
			background-color: var(--background);
			border-radius: 50px;
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--ball);
				translate: 10px 10px;
				border-radius: 50%;
				box-shadow:
					150px 0 var(--ball),
					300px 0 var(--ball);
			}
		}
		& > div:nth-child(2),
		& > div:nth-child(3) {
			--ball: var(--red);
			--background: var(--black);
			translate: 0 -100px;
		}
		& > div:nth-child(3) {
			translate: 0 100px;
		}
	}
</style>
