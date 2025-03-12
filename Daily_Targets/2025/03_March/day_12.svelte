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
		--dark: #5a9f48;
        background-color:var(--light);
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

		& > div {
			position: absolute;
			height: 160px;
			aspect-ratio: 1;
			background-color: var(--light);
			/* opacity: 0.5; */
			border-radius: 50%;
			/* left: 20px; */
			box-shadow: 0 0 0 40px var(--dark);
			&:before,
			&:after {
				content: '';
				position: absolute;
				background-color: var(--light);
				height: 300px;
				width: 30px;
				transform: translate(65px, -70px);
			}
			&:after {
				transform: translate(65px, -70px) rotate(-90deg);
			}
		}
		& > div:nth-child(1) {
			transform: translateX(-100px);
		}
		& > div:nth-child(2) {
			transform: translateX(100px);
		}
	}
</style>

