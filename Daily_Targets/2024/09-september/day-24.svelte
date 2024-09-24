<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		--purple: #9076d8;
		--white: #f3ead2;
        background-color:var(--purple);
		& > div {
			transform: translate(-44px, 0px);
			background-color: var(--white);
			position: absolute;
			height: 200px;
			width: 40px;
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 140px;
				width: 40px;
				background-color: var(--white);
				transform-origin: bottom;
				transform: translate(-6px, -27px) rotate(45deg);
			}
			&:after {
				transform-origin: bottom;
				transform: scaleY(-1) translate(-6px, 53px) rotate(45deg);
			}
		}
	}
</style>

