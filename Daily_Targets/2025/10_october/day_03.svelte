<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #23384b;
		--yellow: #f0cd48;
        background-color:var(--green);
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
			position: absolute;
			height: 100px;
			width: 40px;
			background-color: var(--yellow);
			translate: -30px;
			box-shadow:
				60px 0px var(--yellow),
				120px 0px var(--yellow),
				180px 0px var(--yellow),
				-60px 0px var(--yellow),
				-120px 0px var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 100px;
				background-color: var(--yellow);
				translate: -120px -60px;
				box-shadow:
					240px 0px var(--yellow),
					0px 180px var(--yellow),
					240px 180px var(--yellow);
			}
		}
	}
</style>
