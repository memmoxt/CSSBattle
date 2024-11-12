<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--darkblue: #2d3464;
		--blue: #c0d6e7;
		--red: #d95362;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--darkblue);
		& > div {
			height: 120px;
			width: 120px;
			background-color: var(--blue);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--blue);
				height: 75px;
				width: 160px;
				transform: translate(-20px, 22px);
				border-radius: 62px/70px;
			}
			&:after {
				content: '';
				position: absolute;
				background-color: var(--red);
				height: 60px;
				width: 16px;
				bottom: 30px;
				box-shadow:
					26px 0 0 0 var(--red),
					52px 0 0 0 var(--red),
					78px 0 0 0 var(--red),
					104px 0 0 0 var(--red);
			}
		}
	}
</style>

