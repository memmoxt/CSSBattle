<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fade8b;
		--green: #61a74e;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--yellow);
		& > div {
			position: absolute;
			top: 150px;
			height: 40px;
			width: 400px;
			background-color: var(--green);
			&:before {
				position: absolute;
				content: '';
				right: 160px;
				top: -40px;
				height: 80px;
				aspect-ratio: 1;
				border-radius: 50%;
				box-shadow:
					0 0 0 40px var(--yellow),
					0 0 0 80px var(--green);
				clip-path: polygon(-80px 40px, 180px 40px, 200px 180px, -100px 180px);
			}
			&:after {
				position: absolute;
				content: '';
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--green);
				right: 160px;
				top: -40px;
				height: 80px;
				aspect-ratio: 1;
				border-radius: 50%;
			}
		}
	}
</style>
