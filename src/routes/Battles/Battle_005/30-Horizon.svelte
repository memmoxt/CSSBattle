<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>
<style>
	* {
		margin: 0;
		padding: 0;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: start;
		flex-direction: column;
		align-items: start;

		& > :nth-child(1) {
			height: 50px;
			width: 400px;
			background-color: #f7ec7d;
		}

		& > :nth-child(2) {
			height: 50px;
			width: 400px;
			background-color: #e38f66;
		}

		& > :nth-child(3) {
			height: 100px;
			width: 400px;
			background-color: #aa445f;
		}

		& > :nth-child(4) {
			height: 100px;
			width: 400px;
			background-color: #62306d;
		}
	}
</style>
