<div class="main">
	<div>
		<div></div>
		<div></div>
	</div>
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
		--yellow: #f5e3b5;
		--blue: #469dba;
        background-color:var(--yellow);
		& > div {
            position: absolute;
			height: 180px;
			width: 240px;
            overflow:hidden;
			& > div {
				position: absolute;
				right: -60px;
				top: -60px;
				height: 120px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--yellow);
				box-shadow: 0 0 0 60px var(--blue);
				&:before {
					position: absolute;
					content: '';
					height: 60px;
					width: 240px;
					left: -180px;
					top: 120px;
					background-color: var(--blue);
				}
			}
			& > div:nth-child(2) {
				transform: translateY(180px) scaleY(-1);
			}
		}
	}
</style>

