<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #2f5a76;
		--yellow: #f5bb60;
        background-color:var(--blue);
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
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			transform: rotate(45deg);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 100px;
				background-color: var(--yellow);
				top: 120px;
				box-shadow: 0 -170px 0 0 var(--yellow);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 30px;
				right: 120px;
				background-color: var(--yellow);
				box-shadow: 170px 0 0 0 var(--yellow);
			}
		}
	}
</style>

