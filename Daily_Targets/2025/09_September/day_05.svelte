<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #ca8e75;
		--purple: #414b81;
		--yellow: #feff58;
        background-color:var(--orange);
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
			height: 200px;
			width: 220px;
			background-color: var(--yellow);
			transform: rotate(15deg);
			&:before {
				content: '';
				position: absolute;
				height: 340px;
				width: 120px;
				background-color: var(--purple);
				transform: rotate(60deg);
				translate: 50px -70px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 80px;
				background-color: var(--yellow);
				translate: 70px 70px;
			}
		}
	}
</style>
