<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #4f55a2;
		--yellow: #dcc6a8;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--purple);
		& > div {
			position: absolute;
			height: 95px;
			width: 190px;
			transform: translatey(47px);
			background-color: var(--yellow);
			border-bottom-left-radius: 30px;
			border-bottom-right-radius: 30px;
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 80px;
				width: 30px;
				border-radius: 50px;
				transform: translate(-15px, -65px);
				box-shadow: 0 0 0 10px var(--purple);
				background-color: var(--yellow);
			}
			&:after {
				transform: translate(175px, -65px);
			}
		}
	}
</style>
