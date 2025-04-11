<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #d96c7b;
		--darkred: #8d424d;
		--light: #a4c5bd;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--light);

		& > div {
			height: 140px;
			width: 190px;
			border-top-right-radius: 50px;
			border-top-left-radius: 50px;
			background-color: var(--red);
			overflow: hidden;

			&:before {
				content: '';
				position: absolute;
				height: 140px;
				width: 100px;
				transform: translate(0px);
				background-color: var(--darkred);
				border-top-right-radius: 50px;
				border-top-left-radius: 50px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 20px;
				background-color: var(--red);
				transform: translate(141px, 140px);
				box-shadow: -10px 0 0 0px var(--darkred);
			}
		}
	}
</style>

