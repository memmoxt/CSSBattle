<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--sky: #9ac5ff;
		--blue: #3166ae;
		--white: #ffffff;
		background-color: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			background-color: var(--sky);
			height: 36px;
			width: 133px;
			border-radius: 73px / 22px;
			transform: translateY(63px);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				transform: translate(17px, -103px) rotate(45deg);
				border-bottom-right-radius: 0px;
			}
		}
	}
</style>
