<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #024817;
		--mid: #25834a;
		--light: #48bf7d;
		background: var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			position: absolute;
			height: 160px;
			width: 240px;
			background-color: var(--mid);
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 200px;
			width: 60px;
			background-color: var(--light);
		}
	}
</style>
