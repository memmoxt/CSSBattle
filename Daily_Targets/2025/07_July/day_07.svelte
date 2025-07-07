<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #48bf7d;
		--purple: #32295a;
		background-color: var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;

		& > div {
			height: 280px;
			width: 400px;
			translate: -30px -20px;
			overflow: hidden;
			& > div {
				height: 500px;
				aspect-ratio: 1;
				background-color: var(--green);
				border-radius: 50%;
				translate: 30px 10px;
			}
		}
	}
</style>
