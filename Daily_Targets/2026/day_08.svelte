<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f2eaa8;
		--red: #ee7667;
		--green: #84be8d;
        background-color: var(--yellow);
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
			height: 40px;
			width: 90px;
			background-color: var(--red);
			translate: -120px -90px;
			box-shadow:
				240px 0px var(--red),
				0px 180px var(--green),
				240px 180px var(--green);
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				width: 40px;
				background-color: var(--red);
				translate: 25px 10px;
				box-shadow:
					240px 0px var(--red),
					0px 120px var(--green),
					240px 120px var(--green);
			}

		}
	}
</style>
