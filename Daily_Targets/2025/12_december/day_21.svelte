<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #2f5a76;
		--yellow: #f3ac3c;
        background-color: var(--green);
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
			height: 120px;
			width: 60px;
			background-color: var(--green);
			translate: 0 0;
			border-bottom-left-radius: 20px;
			border-bottom-right-radius: 20px;
			box-shadow: 0 0 0 20px var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				width: 100px;
				background-color: var(--green);
				translate: -20px -20px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				width: 60px;
				background-color: var(--yellow);
				translate: -80px -20px;
				box-shadow:
					0 40px var(--yellow),
					160px 40px var(--yellow),
					160px 0px var(--yellow);
			}
		}
	}
</style>
