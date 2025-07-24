<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #328fc1;
		--brown: #3d2525;
		background-color: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		background-color: var(--red);
		& > div {
			height: 105px;
			width: 50px;
			background-color: var(--brown);
			border-bottom-left-radius: 10px;
			border-bottom-right-radius: 10px;
			&::before {
				content: '';
				position: absolute;
				height: 40px;
				width: 40px;
				background-color: var(--blue);
				translate: 5px 5px;
				border-bottom-left-radius: 20px;
				border-bottom-right-radius: 20px;
			}
		}
	}
</style>
