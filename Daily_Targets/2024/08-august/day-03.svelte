<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #232323;
		--blue: #78b4f3;
		--red: #df7065;
		--white: #f2f2f2;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--black);
		& > div {
            border-top: 75px solid var(--white);
            border-right: 125px solid var(--blue);
            border-bottom: 75px solid var(--red);
            border-left: 125px solid var(--red);
		}
	}
</style>

