<div class="main">
	<div>
		<div></div>
		<div></div>
	</div>
	<div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--white: #ffffff;
		--blue: #328fc1;
		& > div {
			overflow: hidden;
			position: absolute;
			left: 80px;
			height: 180px;
			width: 120px;
			& > div:nth-child(1) {
				height: 40px;
				position: absolute;
				top: 40px;
				left: 40px;
				aspect-ratio: 1;
				box-shadow: 0 0 0 40px var(--blue);
				background-color: var(--white);
				border-radius: 50%;
				z-index: 1;
			}
			& > div:nth-child(2) {
				position: absolute;
				border-radius: 50%;
				top: -15px;
				left: -75px;
				height: 154px;
				aspect-ratio: 1;
				box-shadow: 0 0 0 40px var(--blue);
				clip-path: polygon(131px 99px, 205px 85px, 200px 200px, 0px 200px);
				background-color: var(--white);
			}
		}
		& > div:nth-child(2) {
			left: 200px;
		}
	}
</style>

