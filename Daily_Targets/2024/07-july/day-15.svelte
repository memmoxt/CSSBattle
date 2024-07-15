<div class="main">
	<div><div></div></div>
	<div><div></div></div>
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #b53733;
		--orange: #ea7457;
		background: var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			height: 160px;
			aspect-ratio: 1;
			transform: translate(-95px, 0);
			overflow: hidden;
			& > div {
				height: 160px;
				aspect-ratio: 1;
				background-color: var(--orange);
				transform: translate(50%, 0%);
				border-radius: 50%;
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 150px;
			width: 30px;
			transform: translateX(25px);
			background-color: var(--orange);
		}

		& > div:nth-child(3) {
			position: absolute;
			height: 160px;
			width: 40px;
			transform: translate(85px, 0);
			overflow: hidden;
			& > div {
				height: 160px;
				aspect-ratio: 1;
				background-color: var(--orange);
				transform: translate(-130px, 0%);
				border-radius: 50%;
			}
		}
	}
</style>
