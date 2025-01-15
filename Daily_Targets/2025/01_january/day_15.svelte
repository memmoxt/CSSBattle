<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
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
		--white: #e0e7ff;
		--blue: #4f77ff;
		background-color: var(--white);
		& > div:nth-child(1),
		& > div:nth-child(2) {
			position: absolute;
			top: 0px;
			background-color: var(--blue);
			height: 75px;
			width: 30px;
			&:before {
				position: absolute;
				content: '';
				height: 50px;
				width: 122px;
				background-color: transparent;
				left: -76px;
				top: 55px;
				border-top: 0px solid transparent;
				border-right: 30px solid transparent;
				border-left: 30px solid transparent;
				border-bottom: 30px solid var(--blue);
			}
		}
   		& > div:nth-child(2) {
			top: 225px;
			transform: scaleY(-1);
		}

	
	}
</style>

