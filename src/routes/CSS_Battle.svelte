<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--rose: #ec007b;
		--pink: #f7bed9;
		background-color: var(--pink);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 50px;
			width: 200px;
			background-color: var(--rose);
			transform: translate(-100px, -35px);
			box-shadow:
				250px 0 var(--rose),
				200px 70px var(--rose),
				-50px 70px var(--rose);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 150px;
				transform: translate(150px, -50px);
				box-shadow: -50px 170px var(--rose);
				background-color: var(--rose);
			}
		}
	}
</style>
