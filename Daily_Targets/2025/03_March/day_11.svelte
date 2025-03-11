<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #323130;
		--blue: #00b0c8;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 80px;
			width: 400px;
			background-color: var(--blue);
			/* opacity: 0.5; */
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				width: 160px;
				background-color: var(--blue);
				top: -110px;
				left: 120px;
				box-shadow: 0 220px var(--blue);
			}
			&:after {
				content: '';
				position: absolute;
				background-color: var(--black);
				height: 40px;
				width: 80px;
				top: 20px;
				left: 160px;
			}
		}
	}
</style>

