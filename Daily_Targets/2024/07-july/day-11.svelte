<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #024817;
		--green: #176c36;
		--light: #48bf7d;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--green);
		& > div {
			position: absolute;
			top: 210px;
			border-top: 50px solid var(--light);
			border-right: 40px solid transparent;
			border-bottom: 50px solid transparent;
			border-left: 40px solid transparent;
		}
		& > div:nth-child(2) {
			transform: translate(-110px, -110px) rotate(90deg);
		}

		& > div:nth-child(3) {
			transform: translate(110px, -110px) rotate(-90deg);
		}

		& > div:nth-child(4) {
			transform: translate(0px, -220px) rotate(180deg);
		}
		& > div:nth-last-child(1) {
			height: 80px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--dark);
			transform: translate(0px, -100px);
			border: none;
		}
	}
</style>
