<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #6592cf;
		--yellow: #f7cb71;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			height: 200px;
			aspect-ratio: 1;
			background-color: var(--blue);
			/* opacity: 0; */
			border-radius: 50%;
			box-shadow: 0 0 0 20px var(--yellow);
		}
		& > div:nth-child(2),
		& > div:nth-child(2):before {
			position: absolute;
			height: 180px;
			width: 50px;
			background-color: var(--yellow);
			/* opacity: 0.5; */
			border-radius: 50%;
		}
        &>div:nth-child(2):before{
            content:'';
            transform:rotate(90deg);
        }
	}
</style>

