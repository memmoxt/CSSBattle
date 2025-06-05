<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #394257;
		--light: #eed9d9;
        background-color:var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 260px;
			aspect-ratio: 1;
			background-color: var(--dark);
			transform: translate(0px, 80px);
			border-radius: 50%;
			box-shadow: 0 0 0 40px var(--light);
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				width: 100px;
				background-color: var(--dark);
				transform: translate(80px, -30px);
				box-shadow: 0 0 0 40px var(--light);
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				width: 400px;
				transform: translate(-70px, 130px);
				box-shadow: 0px 40px 0 10px var(--dark);
				background-color: var(--light);
			}
		}
	}
</style>
