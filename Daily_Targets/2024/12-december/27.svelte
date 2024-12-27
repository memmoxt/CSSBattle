<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #61a74e;
		--white: #eff8fe;
        background-color:var(--green);
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
			top: 70px;
			height: 40px;
			width: 400px;
			background-color: var(--white);
			box-shadow: 0 120px 0 0 var(--white);
			&:before {
				position: absolute;
				content: '';
				top: -40px;
				left: 120px;
				height: 240px;
				width: 40px;
				box-shadow: 120px 0 0 0 var(--white);
				background-color: var(--white);
			}
		}
	}
</style>

