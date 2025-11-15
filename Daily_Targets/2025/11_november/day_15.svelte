<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fad98c;
		--blue: #89b3ec;
		--black: #2a2828;
		--dark: #3c5a84;
		background-color: var(--yellow);
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
			height: 190px;
			width: 300px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				width: 70px;
				background-color: var(--dark);
				translate: 130px;
				clip-path: polygon(0 0, 40px 0px, 40px 130px, 80px 130px, 80px 180px, 0px 180px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 280px;
				translate: 10px;
				clip-path: polygon(
					0 0,
					100% 0px,
					100% 100%,
					180px 100%,
					180px 30px,
					100px 30px,
					100px 100%,
					0 100%
				);
				background-color: var(--black);
			}
		}
	}
</style>
