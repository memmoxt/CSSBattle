<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		--white: #f5f5f5;
		--blue: #6592cf;
        background-color:var(--blue);

		& > div:nth-child(1) {
			height: 180px;
			width: 25.4px;
			background-color: var(--white);
			transform: translateX(-112px);
			box-shadow:
				75px 0 0 var(--white),
				150px 0 0 var(--white),
				225px 0 0 var(--white);
		}
		& > div:nth-child(2) {
			height: 25px;
			width: 100px;
			background-color: var(--white);
			position: absolute;
			top: 215px;
			box-shadow:
				-74.9px -155px 0 var(--white),
				74.9px -155px 0 var(--white);
		}
	}
</style>

