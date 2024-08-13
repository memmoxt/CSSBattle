<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--pink: #d96e9f;
		--purple: #6255aa;
		background-color: var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 220px;
			width: 150px;
			background-color: var(--pink);
			&:before,
			&:after {
				content: '';
				position: absolute;
				background-color: var(--purple);
			}
			&:before {
				height: 160px;
				width: 60px;
				transform: translate(30px, 30px);
			}
			&:after {
				height: 60px;
				width: 30px;
				transform: translate(90px, 130px);
			}
		}
	}
</style>
