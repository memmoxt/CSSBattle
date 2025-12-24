<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #302562;
		--blue: #0098d1;
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
			height: 150px;
			width: 220px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 200px;
				width: 80px;
				translate: 70px -25px;
				background-color: var(--blue);
			}
			&:after {
				content: '';
				position: absolute;
				height: 50px;
				width: 170px;
				background-color: var(--blue);
				translate: 25px -85px;
				box-shadow: 0 270px var(--blue);
			}
		}
	}
</style>
