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
		--black: #41434b;
		--white: #ffffff;
		--red: #d95f5b;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;

		& > div:nth-child(1),
		div:nth-child(2) {
			position: absolute;
			translate: -90px -30px;
			border-top-left-radius: 50px;
			border-top-right-radius: 50px;
			border-bottom-left-radius: 50px;
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				translate: 15px 35px;
				aspect-ratio: 1;
				background-color: var(--black);
				border-radius: 50%;
			}
		}
		& > div:nth-child(2) {
			border-bottom-left-radius: 0px;
			border-bottom-right-radius: 50%;
			translate: 90px -30px;
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 60px;
			width: 80px;
			translate: 0px 50px;
			clip-path: polygon(0 0, 100% 0px, 50% 100%);
			background-color: var(--red);
		}
	}
</style>
