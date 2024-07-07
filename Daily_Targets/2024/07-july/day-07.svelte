<div class="main">
	<div class="circles"></div>
	<div class="center-dot"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #feff58;
		--orange: #f48b26;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: end;
		overflow: hidden;
		position: absolute;
        background:var(--orange);
		& > .circles {
			height: 500px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			border-radius: 50%;
			transform: translate(325px, 100px);
			&:before {
				content: '';
				position: absolute;
				height: 500px;
				width: 500px;
				border-radius: 50%;
				background-color: var(--yellow);
				transform: translate(-130%, 0);
			}
		}

		& > .center-dot {
			position: absolute;
			height: 160px;
			border-top-left-radius: 25px;
			border-top-right-radius: 25px;
			width: 50px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
                border-radius:50%;
				aspect-ratio: 1;
				background-color: var(--yellow);
				transform: translate(0px, -65px);
			}
		}
	}
</style>

