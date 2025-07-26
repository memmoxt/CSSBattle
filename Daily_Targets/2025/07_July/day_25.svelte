<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fade8b;
		--gray: #556d7f;
		--red: #d24444;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 72px;
			aspect-ratio: 1;
			border-radius: 20px/20px;
			background-color: var(--red);
			translate: 72px -26px;
			box-shadow:
				-72px 72px var(--gray),
				-92px -20px var(--gray);
		}
	}
</style>
