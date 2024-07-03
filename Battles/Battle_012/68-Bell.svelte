<div class="main">
	<div class="balls"></div>
	<div class="bell"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #e08027;
		--yellow: #f2ad43;
		--brown: #824b20;
		--black: #191919;
	}

	.main {
		height: 300px;
		width: 400px;
		background-color: var(--black);
		display: flex;
		justify-content: center;
		align-items: center;
		& > .bell {
			height: 120px;
			border-radius: 60px 60px 10px 10px;
			width: 120px;
			background: var(--orange);
			z-index: 1;
		}
		& > .balls {
			position: absolute;
			height: 120px;
			width: 120px;
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 50px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--yellow);
				transform: translate(35px, -24px);
			}
			&:after {
				top: 120px;
				background-color: var(--brown);
			}
		}
	}
</style>
