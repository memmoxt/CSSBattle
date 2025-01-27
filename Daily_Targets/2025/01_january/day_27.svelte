<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--blue: #469dba;
		--yellow: #f5e3b5;
        background-color:var(--blue);
		& > div {
			height: 30px;
			width: 60px;
			background-color: var(--yellow);
			transform: translate(-130px);
			box-shadow:
				0px -120px 0 var(--yellow),
				0px 120px 0 var(--yellow);
			&:before {
				position: absolute;
				content: '';
				height: 30px;
				width: 120px;
				background-color: var(--yellow);
				top: 60px;
				box-shadow: 0 -120px var(--yellow);
			}
		}
		& > div:nth-child(2) {
			transform: translate(130px) scale(-1);
		}
	}
</style>

