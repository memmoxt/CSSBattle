<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #183539;
		--yellow: #ebe77e;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
        background-color:var(--green);
		& > div:nth-child(1) {
			position: absolute;
			height: 225px;
			width: 100px;
			top: 60px;
			background-color: var(--yellow);
			overflow: hidden;
			z-index: 2;
			&:before {
				position: absolute;
				content: '';
				top: 135px;
				left: -25px;
				background-color: var(--green);
				height: 50px;
				aspect-ratio: 1;
				border-radius: 50%;
			}
			&:after {
				position: absolute;
				content: '';
				top: 45px;
				background-color: var(--green);
				height: 15px;
				width: 50px;
			}
		}
		& > div:nth-child(2) {
			top: 15px;
			position: absolute;
			height: 100px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--yellow);
			z-index: 1;
		}
	}
</style>

