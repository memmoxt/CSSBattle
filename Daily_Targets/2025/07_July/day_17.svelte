<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--azure: #6592cf;
		--blue: #243d83;
		--white: #ffffff;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 120px;
			width: 100px;
			background-color: var(--azure);
			translate: -20px 30px;
			box-shadow: 40px -60px var(--azure);
			&:before {
				content: '';
				position: absolute;
				height: 72px;
				width: 12px;
				background-color: var(--white);
				translate: -12px 60px;
				box-shadow: 112px -72px var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 12px;
				width: 72px;
				background-color: var(--white);
				translate: -12px 120px;
				box-shadow: 52px -132px var(--white);
			}
		}
	}
</style>
