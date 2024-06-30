<div class="main">
	<div class="base">
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
	<div class="circle-cut">
		<div class="circles"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f9e492;
		--black: #191919;
		--blue: #4f77ff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--black);
		& > .base {
			height: 150px;
			aspect-ratio: 1;
			border-radius: 50%;
			overflow: hidden;
			display: grid;
			grid-template-columns: repeat(2, 1fr);
			grid-template-rows: repeat(4, 1fr);
			gap: 10px;
			& > div {
				background-color: var(--blue);
			}
		}
		& > .circle-cut {
			position: absolute;
			height: 150px;
			aspect-ratio: 1;
			overflow: hidden;
			& > .circles {
				position: absolute;
				height: 210px;
				border-radius: 50%;
				aspect-ratio: 1;
				transform: translate(30px, -30px);
				border: 10px solid var(--black);
				&:before {
					content: '';
					position: absolute;
					height: 210px;
					border-radius: 50%;
					aspect-ratio: 1;
					transform: translate(-130px, -10px);
					border: 10px solid var(--black);
				}
			}
		}
	}
</style>
