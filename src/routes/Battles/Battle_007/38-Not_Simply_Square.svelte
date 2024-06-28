<div class="main">
	<div></div>
</div>
<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		background: #293462;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: start;
		align-items: center;

		& > div {
			height: 200px;
			aspect-ratio: 1;
			background-color: #fff1c1;
			align-self: self-start;

			&:before {
				content: '';
				position: absolute;
				height: 150px;
				width: 100px;
				background-color: #fe5f55;
				border-bottom: 50px solid #a64942;
				transform: translate(200px, 0%);
			}

			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 150px;
				background-color: #fe5f55;
				border-right: 50px solid #a64942;
				transform: translate(0%, 200px);
			}
		}
	}
</style>
