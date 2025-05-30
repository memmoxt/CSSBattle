<div class="main">
	<div class="top"></div>
	<div class="bottom"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #594c94;
		--green: #bfe33a;
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
		& > .top,
		& > .bottom {
			position: absolute;
			height: 80px;
			width: 80px;
			background-color: var(--green);
			transform: translate(-140px, -90px);
			border-top-left-radius: 10px;
			border-top-right-radius: 10px;
			border-bottom-left-radius: 10px;
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 60px;
				background-color: var(--green);
				transform: translate(80px, 20px);
				border-top-right-radius: 10px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				width: 40px;
				background-color: var(--green);
				transform: translate(140px, 40px);
				border-top-right-radius: 10px;
				box-shadow:
					20px 40px var(--green),
					20px 60px var(--green);
			}
		}
		& > .bottom {
			transform: translate(140px, 90px) scale(-1);
		}
	}
</style>
