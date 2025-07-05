<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f0cd48;
		--white: #ffffff;
		--black: #394257;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		background-color: var(--yellow);
		& > div {
			height: 60px;
			width: 340px;
			background-color: var(--white);
			border-radius: 10px/10px;
			box-shadow: 0 0 0 10px var(--black);
			&::before {
				content: '';
				position: absolute;
				height: 44px;
				width: 10px;
				background-color: var(--black);
				translate: 14px 8px;
			}
		}
	}
</style>
