<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f4da64;
		--red: #e25c57;
        background-color: var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--red);
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 20px;
				background-color: var(--red);
				translate: -44px -64px;
				transform: rotate(-45deg);
				box-shadow: 0px 180px var(--red);
			}
			&:after {
				translate: 83px -64px;
				transform: rotate(45deg);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 30px;
			translate: -90px;
			aspect-ratio: 1;
			background-color: var(--red);
			border-radius: 50%;
			box-shadow:
				180px 0 var(--red),
				90px 90px var(--red),
				90px -90px var(--red);
		}
	}
</style>
