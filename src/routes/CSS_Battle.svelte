<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #3a335a;
		--blue: #b6ebe7;
		background-color: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			position: absolute;
			height: 108px;
			width: 36px;
			background-color: var(--purple);
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 200px;
				translate: -164px -78px;
				background-color: var(--purple);
			}
			&:after {
				translate: 0px 126px;
			}
		}
	}
</style>
