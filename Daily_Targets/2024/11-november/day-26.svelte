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
		--purple: #6255aa;
		--pink: #de88af;
        background-color:var(--purple);
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
		& > div:nth-child(2) {
			position: absolute;
			height: 120px;
			aspect-ratio: 1;
			background-color: var(--pink);
			border-radius: 50%;
			border-bottom-right-radius: 0;
			transform: translateX(-75px);
			&:before {
				position: absolute;
				content: '';
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--purple);
				border-radius: 50%;
				top: 30px;
				left: 30px;
			}
		}
		& > div:nth-child(2) {
			transform: translateX(75px) scaleX(-1);
		}
		& > div:nth-child(3) {
			position: absolute;
			height: 90px;
			width: 30px;
			background-color: var(--purple);
			box-shadow: 0 0 0 30px var(--pink);
			bottom: 0px;
		}
	}
</style>

