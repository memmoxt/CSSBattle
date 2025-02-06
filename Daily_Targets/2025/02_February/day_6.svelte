<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #d95362;
		--blue: #2d3464;
        background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        
		& > div:nth-child(1) {
			position: absolute;
			top: 60px;
			left: 80px;
			border-radius: 50%;
			border-top: 120px solid var(--blue);
			border-right: 120px solid var(--red);
			border-bottom: 120px solid var(--blue);
			border-left: 120px solid var(--blue);
			transform: rotate(-45deg);
			&:before {
				position: absolute;
				content: '';
				top: -42px;
				left: -42px;
				height: 84px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--blue);
				box-shadow: 0 0 0 38px var(--red);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			bottom: 240px;
			height: 160px;
			aspect-ratio: 1;
			background-color: var(--red);
			border-radius: 50%;
			box-shadow: 0 0 0 40px var(--blue);
			clip-path: polygon(80px 100px, 210px 100px, 210px 200px, 80px 210px);
		}
	}
</style>

