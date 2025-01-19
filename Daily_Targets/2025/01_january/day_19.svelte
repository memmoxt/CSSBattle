<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--blue: #328fc1;
		--yellow: #fade8b;
		background-color: var(--blue);
		& > div {
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			&:before,
			&:after {
				position: absolute;
				content: '';
				height: 140px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--yellow);
				top: -70px;
				left: -70px;
			}
			&:after {
				top: 230px;
				left: 330px;
			}
		}
	}
</style>

