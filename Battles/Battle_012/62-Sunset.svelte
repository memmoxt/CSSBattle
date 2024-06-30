<div class="main">
	<div class="window">
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5dbcf9;
		--black: #191919;
		--amber: #f2ad43;
		--yellow: #fff58f;
		--orange: #e08027;
		--brown: #824b20;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		overflow: visible;
		background-color: var(--black);
		& > .window {
			height: 200px;
			width: 150px;
			border-radius: 150px 150px 40px 40px;
			overflow: hidden;
			background-color: var(--amber);
			& > div:nth-child(1) {
				height: 60px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(45px, 90px);
				background-color: var(--yellow);
			}
			& > div:nth-child(2) {
				height: 200px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(-100px, 40px);
				background-color: var(--orange);
				&:before {
					content: '';
					position: absolute;
					height: 200px;
					aspect-ratio: 1;
					border-radius: 50%;
					transform: translate(150px, 0px);
					background-color: var(--brown);
				}
			}
		}
	}
</style>
