<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #6d62ba;
		--blue: #a1e6e4;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		background-color: var(--purple);
		& > div {
			height: 90px;
			aspect-ratio: 1;
			background-color: var(--blue);
			border-radius: 50%;
			&:before {
				position: absolute;
				content: '';
				height: 90px;
				width: 30px;
				left: 95px;
				box-shadow: 180px 0 0 var(--blue);
				background-color: var(--blue);
			}
			&:after {
				position: absolute;
				content: '';
				height: 30px;
				width: 90px;
				top: 45px;
				background-color: var(--blue);
				box-shadow: 0 180px 0 var(--blue);
			}
		}
	}
</style>

