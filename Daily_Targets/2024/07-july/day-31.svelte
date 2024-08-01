<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #edaf38;
		--green: #7f7f24;
		--white: #ffffcd;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--yellow);
		& > div:nth-child(1) {
			height: 160px;
			width: 260px;
			clip-path: polygon(0px 120px, 220px 0, 260px 0, 260px 160px, 0 160px);
			transform: translate(-20px, -20px);
			background-color: var(--green);
			&:before {
				position: absolute;
				content: '';
				height: 60px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--white);
				box-shadow: 80px 0px 0 var(--white);
				top: 80px;
				left: 100px;
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			transform: translate(130px, 40px);
			height: 40px;
			aspect-ratio: 1;
			background-color: var(--green);
			box-shadow: -40px 40px 0 var(--green);
		}
	}
</style>
