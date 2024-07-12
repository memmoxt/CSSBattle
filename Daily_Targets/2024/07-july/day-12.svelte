<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #243d83;
		--light: #6592cf;
		background-color: var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;

		& > div {
			height: 100px;
			width: 250px;
			clip-path: polygon(0% 0%, 30% 0%, 50% 100%, 70% 0%, 100% 0%, 100% 100%, 0% 100%);
			background-color: var(--light);
		}
		& > div:nth-child(1) {
			align-self: start;
			justify-self: start;
		}
		& > div:nth-child(2) {
			align-self: end;
			justify-self: end;
			transform: scaleY(-1);
		}
	}
</style>
