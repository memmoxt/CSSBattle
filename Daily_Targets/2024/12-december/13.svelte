<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #61a74e;
		--yellow: #fade8b;
        background-color:var(--green);
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
			position: absolute;
			top: 30px;
			height: 180px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 50%;
			&:before {
				position: absolute;
				content: '';
				background-color: var(--green);
				height: 120px;
				width: 40px;
				top: 30px;
				left: 70px;
				border-radius: 50px/50px;
			}
			&:after {
				position: absolute;
				content: '';
				background-color: var(--yellow);
				height: 180px;
				width: 60px;
				top: 151px;
				left: -18px;
				transform-origin: top;
				transform: rotate(-60deg);
				border-top-right-radius: 60px;
				border-bottom-left-radius: 60px;
			}
		}
	}
</style>

