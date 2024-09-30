<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f3ead2;
		--yellow: #eac049;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap-reverse;
		flex-direction: column;
		& > div:nth-child(2) {
			position: absolute;
			border-top: 60px solid var(--white);
			border-right: 60px solid var(--yellow);
			border-bottom: 60px solid var(--yellow);
			border-left: 60px solid var(--white);
		}
		& > div:nth-child(1) {
			height: 200px;
			aspect-ratio: 1;
			background-color: var(--yellow);
		}
	}
</style>

