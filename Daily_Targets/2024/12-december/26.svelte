<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #5393bd;
		--yellow: #fae29e;
        background-color:var(--blue);
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
			height: 30px;
			width: 200px;
			background-color: var(--yellow);
			/* opacity: 0.5; */
			position: absolute;
			bottom: 50px;
			&:before,
			&:after {
				content: '';
				height: 30px;
				width: 200px;
				position: absolute;
				bottom: 85px;
				left: -85px;
				background-color: var(--yellow);
				transform: rotate(90deg);
			}
			&:after {
				left: -5px;
				bottom: 60px;
				width: 164px;
				transform: rotate(45deg);
			}
		}
	}
</style>

