<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--light: #bfe33a;
		--green: #5a9f48;
		background-color: var(--light);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: start;
		align-items: start;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			top: 70px;
			left: 20px;
			height: 160px;
			width: 160px;
			border-radius: 50%;
			background-color: var(--light);
			box-shadow: 0 0 0 40px var(--green);
			/* opacity: 0.5; */
			clip-path: polygon(
				-20px -50px,
				200px -50px,
				200px 61px,
				10px 61px,
				0px 80px,
				0px 300px,
				-20px 300px
			);

			&:before {
				content: '';
				position: absolute;
				height: 150px;
				top: 80px;
				width: 20px;
				background-color: var(--green);
				left: -20px;
			}
		}
		& > div:nth-child(2) {
			transform: scale(-1);
			left: 220px;
			top: 70px;
			clip-path: polygon(
				-20px -50px,
				200px -50px,
				200px 60px,
				10px 60px,
				0px 80px,
				0px 300px,
				-20px 300px
			);
		}
	}
</style>

