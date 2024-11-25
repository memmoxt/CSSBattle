<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #e8ad6d;
		--purple: #7e6293;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			left: 120px;
			top: 30px;
			height: 240px;
			width: 60px;
			background-color: var(--purple);
			border-radius: 50px/50px;
			&:before {
				position: absolute;
				content: '';
				background-color: var(--purple);
				height: 60px;
				width: 160px;
				border-radius: 50px/50px;
			}
			&:after {
				top: 90px;
				position: absolute;
				content: '';
				background-color: var(--purple);
				height: 60px;
				width: 120px;
				border-radius: 50px/50px;
			}
		}
	}
</style>

