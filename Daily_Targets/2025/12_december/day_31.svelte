<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #9d92c8;
		--yellow: #f9ddc6;
        background-color: var(--purple);
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
			width: 320px;
			background-color: var(--yellow);
			translate: -0px -70px;
			box-shadow: 0px 140px var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 40px;
				background-color: var(--yellow);
				translate: 220px 40px;
				box-shadow:
					-160px -140px var(--yellow),
					-160px 140px var(--yellow);
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--purple);
				translate: 60px;
				box-shadow:
					160px 0 var(--purple),
					160px 140px var(--purple),
                    0px 140px var(--purple);
			}
		}
	}
</style>
