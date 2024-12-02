<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #e0e7ff;
		--red: #d96c7b;
		--green: #0b2429;
        background-color:var(--white);
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
		& > div:nth-child(2),
		& > div:nth-child(3),
		& > div:nth-child(4) {
			position: absolute;
			top: 40px;
			left: 130px;
			height: 100px;
			width: 60px;
			background-color: var(--red);
			clip-path: polygon(
				0 40px,
				20px 40px,
				20px 20px,
				20px 20px,
				40px 20px,
				40px 0,
				60px 0,
				60px 60px,
				40px 60px,
				40px 80px,
				20px 80px,
				20px 100px,
				0 100px
			);
			/* opacity: 0.5; */
		}
		& > div:nth-child(2) {
			left: 210px;
			transform: scaleX(-1);
		}
		& > div:nth-child(3) {
			top: 160px;
			transform: scaleY(-1);
		}
		& > div:nth-child(4) {
			top: 160px;
			left: 210px;
			transform: scale(-1);
		}
		& > div:nth-child(5) {
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--green);
			/* opacity: 0.5; */
			clip-path: polygon(
				0px 20px,
				20px 20px,
				20px 0px,
				40px 0px,
				40px 20px,
				60px 20px,
				60px 40px,
				40px 40px,
				40px 60px,
				20px 60px,
				20px 40px,
				0px 40px
			);
		}
	}
</style>

