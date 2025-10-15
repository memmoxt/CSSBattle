<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #8e2c88;
		--pink: #eec8ea;
        background-color: var(--pink);
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
			translate: 38px -105px;
			height: 60px;
			width: 295px;
			background-color: var(--purple);
			box-shadow:
				0 105px var(--purple),
				0 210px var(--purple);
			&:before {
				content: '';
				position: absolute;
				height: 270px;
				width: 60px;
				background-color: var(--purple);
				translate: -75px 0px;
                box-shadow: 310px 0 var(--purple);
			}
		}
	}
</style>
