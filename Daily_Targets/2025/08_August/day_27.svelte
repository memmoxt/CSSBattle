<div class="main">
	<div class="center"></div>
	<div class="side"></div>
	<div class="ball"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--gray: #3f4869;
		--red: #e25c57;
		background-color: var(--gray);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
	}
	.center {
		position: absolute;
		height: 140px;
		aspect-ratio: 1;
		background-color: var(--red);
		border-radius: 50%;
	}
	.side {
		position: absolute;
		height: 80px;
		aspect-ratio: 1;
		background-color: var(--gray);
		border-radius: 50%;
		&:before {
			content: '';
			position: absolute;
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--gray);
			clip-path: polygon(70px 0, 142px 0, 142px 90px, 70px 90px);
			translate: -30px -30px;
		}
		&:after {
			content: '';
			position: absolute;
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--red);
			clip-path: polygon(80px 0, 142px 0, 142px 80px, 80px 80px);
			translate: -30px -30px;
		}
	}
	.ball {
		position: absolute;
		height: 80px;
		border-radius: 50%;
		aspect-ratio: 1;
		background-color: var(--gray);
	}
</style>
