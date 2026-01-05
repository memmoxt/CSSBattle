<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #efeb99;
		--purple: #8647e6;
		background-color: var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;

		& > div {
			height: 170px;
			width: 56px;
			background-color: var(--yellow);
			translate: -168px -65px;
			box-shadow:
				112px 0 var(--yellow),
				224px 0 var(--yellow),
				336px 0 var(--yellow),
				56px 130px var(--yellow),
				168px 130px var(--yellow),
				280px 130px var(--yellow);
		}
	}
</style>
