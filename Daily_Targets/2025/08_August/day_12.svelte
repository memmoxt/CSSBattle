<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		--purple: #7e6293;
		--white: #ffffff;
        background-color:var(--purple);
		& > div {
			height: 120px;
			width: 90px;
			background-color: var(--white);
			box-shadow: 160px 80px var(--white);
			translate: -80px -40px;
			border-radius: 54px/54px;
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 30px;
				border-radius: 20px/20px;
				background-color: var(--purple);
				translate: 30px 30px;
				box-shadow: 160px 80px var(--purple);
			}
			&:after {
				content: '';
				position: absolute;
				height: 200px;
				width: 30px;
				background-color: var(--white);
				transform: skewX(-15deg) translateX(110px);
			}
		}
	}
</style>
