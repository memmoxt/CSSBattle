<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #ffffff;
		--black: #000000;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 160px;
			width: 120px;
			background-color: var(--black);
			transform: translateX(-30px);
			&:before {
				content: '';
				position: absolute;
				height: 120px;
				width: 80px;
				background-color: var(--white);
				transform: translate(20px, 20px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				width: 50px;
				background-color: var(--black);
				transform: translate(50px, 30px);
				box-shadow: 0 60px 0 0 var(--black);
			}
		}
		& > div:nth-child(2) {
			transform: scaleX(-1) translateX(-30px);
		}
	}
</style>

