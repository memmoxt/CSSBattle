<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f7ec7d;
		--blue: #243d83;
		--white: #ffffff;
        background-color:var(--yellow);
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
			position: absolute;
			height: 280px;
			width: 120px;
			background-color: var(--blue);
			border-radius: 60px;
		}
		& > div:nth-child(2) {
			transform: rotate(90deg);
			&:before {
				position: absolute;
				content: '';
				height: 60px;
				aspect-ratio: 1;
				border-radius: 50%;
				box-shadow: 0px 160px var(--white);
				background-color: var(--white);
				transform: translate(30px, 30px);
			}
		}
	}
</style>
