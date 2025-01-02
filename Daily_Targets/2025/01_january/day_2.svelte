<div class="main">
	<div></div>
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
		overflow: hidden;
		position: absolute;
		--blue: #2f5a76;
		--yellow: #f5bb60;
        background-color:var(--blue);
		& > div {
			position: absolute;
			height: 90px;
			width: 30px;
			background-color: var(--yellow);
			transform: translateX(-30px);
			box-shadow: 60px 0 0 0 var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 90px;
				background-color: var(--yellow);
				top: -60px;
				box-shadow: 0 180px 0 0 var(--yellow);
			}
		}
		& > div:nth-child(1) {
			left: 65px;
		}
		& > div:nth-child(2) {
			right: 65px;
		}
	}
</style>

