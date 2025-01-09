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
		--yellow: #fade8b;
		--green: #61a74e;
        background-color:var(--yellow);
		& > div:nth-child(1) {
			position: absolute;
			top: 40px;
			right: 145px;
			height: 165px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 50%;
			box-shadow: 0 0 0 40px var(--green);
			clip-path: polygon(45px 60px, 250px 60px, 250px 250px, 85px 225px, 85px 165px, 45px 165px);
		}
		& > div:nth-child(2),
		div:nth-child(3) {
			position: absolute;
			height: 40px;
			left: 255px;
			bottom: 205px;
			/* opacity: 0.5; */
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 50%;
			box-shadow: 0 0 0 40px var(--green);
		}
		& > div:nth-child(3) {
			&:before {
				content: '';
				position: absolute;
				height: 185px;
				width: 40px;
				background-color: var(--green);
				top: -190px;
			}
			left: 105px;
			bottom: 55px;
		}
	}
</style>

