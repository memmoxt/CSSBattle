<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--grey: #2f434e;
		--yellow: #f8b140;
		--orange: #cf6939;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		background-color: var(--grey);
		& > div {
			content: '';
			height: 130px;
			translate: 0px -75px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--yellow);
			box-shadow: 0 150px var(--orange);
			&:before {
				position: absolute;
				content: '';
				background-color: var(--yellow);
				height: 100px;
				aspect-ratio: 1;
				translate: 15px 90px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--yellow);
				translate: 35px 110px;
				box-shadow: 0 0 0 10px var(--orange);
			}
		}
	}
</style>
