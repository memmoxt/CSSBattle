<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--gray: #4c455b;
		--red: #d96c7b;
		--white: #f3ead2;
		background-color: var(--gray);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			position: absolute;
			height: 100px;
			width: 140px;
			background-color: var(--red);
			translate: 0 35px;
			box-shadow: 0 0 0 30px var(--white);
			clip-path: polygon(-30px 0px, 180px 0px, 180px 135px, -30px 135px);
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 140px;
			aspect-ratio: 1;
			border-radius: 50%;
			translate: 0 -15px;
			background-color: var(--white);
			box-shadow: 0 0 0 30px var(--red);
			clip-path: polygon(-30px -30px, 200px -30px, 200px 70px, -30px 70px);
		}
	}
</style>
