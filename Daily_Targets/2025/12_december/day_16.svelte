<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--rose: #c06c88;
		--purple: #411c56;
		--blue: #b7d7cd;
        background-color: var(--rose);
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
			height: 160px;
			width: 240px;
			background-color: var(--purple);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 60px;
				background-color: var(--blue);
				translate: 20px 20px;
				box-shadow:
					140px 0 var(--blue),
					80px 80px var(--blue);
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 40px;
				background-color: var(--blue);
				translate: 100px 20px;
				box-shadow:
					-80px 80px var(--blue),
					80px 60px var(--blue);
			}
		}
	}
</style>
