<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fade8b;
		--orange: #d08825;
		--blue: #2d3464;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
        background-color:var(--blue);
		& > div:nth-child(1) {
			position: absolute;
			top: 85px;
			left: 200px;
			height: 130px;
			width: 130px;
			background-color: var(--yellow);
			box-shadow: -200px 0 var(--yellow);
			&:before {
				position: absolute;
				content: '';
				height: 100px;
				width: 141px;
				top: -100px;
				left: -200px;
				background-color: var(--orange);
				box-shadow:
					259px 0 var(--orange),
					259px 230px var(--orange),
					0px 230px var(--orange);
			}
		}
	}
</style>

