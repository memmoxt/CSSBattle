<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #434b92;
		--yellow: #f3ac3c;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 300px;
			width: 190px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 230px;
				transform: translate(-20px, 25px);
				background-color: var(--yellow);
				box-shadow:
					0 100px 0 0 var(--yellow),
					0 200px 0 0 var(--yellow);
			}
		}
	}
</style>

