<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--gray: #2f434e;
		--orange: #cf6939;
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

		& > div {
			height: 70px;
			width: 110px;
			translate: -130px -30px;
			background-color: var(--orange);
			box-shadow: 50px 30px var(--orange),
                100px 60px var(--orange),
                160px 0 var(--orange),
                210px 30px var(--orange),
                260px 60px var(--orange);
		}
	}
</style>
