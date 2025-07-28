<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #ebe77e;
		--purple: #7e6293;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 180px;
			aspect-ratio: 1;
			background-color: var(--purple);
			border-radius: 50%;
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				border-radius: 50px/50px;
				box-shadow:
					0 0 0 20px var(--purple),
					0 0 0 40px var(--yellow);
				translate: 60px 60px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 20px;
				background-color: var(--purple);
				translate: 80px 30px;
			}
		}
	}
</style>
