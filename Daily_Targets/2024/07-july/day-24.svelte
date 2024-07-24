<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--orange: #edaf38;
		--green: #7f7f24;
		--yellow: #ffffcd;
		background: var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 120px;
			width: 280px;
			background-color: var(--yellow);
			&:before,
			&:after {
				position: absolute;
				content: '';
				width: 280px;
				height: 40px;
				border-radius: 50%;
				background-color: var(--green);
				transform: translateY(-20px);
			}
			&:after {
				background-color: var(--yellow);
				transform: translateY(100px);
			}
		}
	}
</style>
