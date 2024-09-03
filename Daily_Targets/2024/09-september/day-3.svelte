<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #c64f4f;
		--white: #f3f3f3;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			background-color: var(--red);
			height: 50px;
			aspect-ratio: 1;
			box-shadow:
				-100px 0 0 var(--red),
				100px 0 0 var(--red),
				-50px 50px 0 var(--red),
				-50px -50px 0 var(--red),
				50px 50px 0 var(--red),
				0px 100px 0 var(--red),
				50px -50px 0 var(--red),
				100px -100px 0 var(--red),
				-100px -100px 0 var(--red),
				150px -50px 0 var(--red),
				-150px -50px 0 var(--red);
		}
	}
</style>

