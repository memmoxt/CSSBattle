<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #62306d;
		--yellow: #f7ec7d;
		--orange: #e38f66;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 200px;
			aspect-ratio: 1;
			background-color:var(--yellow);
			border-radius: 50%;
			display: flex;
			justify-content: center;
			position: relative;
            overflow: hidden;
			& > div {
				height: 50px;
				width: 50px;
				background-color: var(--orange);
				&:before {
					content: '';
					position: absolute;
					height: 120px;
					aspect-ratio: 1;
					background-color: var(--purple);
					border-radius: 50%;
					top: 40px;
					left: 40px;
				}
			}
		}
	}
</style>

