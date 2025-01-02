<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #3f9461;
		--white: #ffffff;
		background-color: var(--green);
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
			height: 180px;
			width: 320px;
			background-color: var(--white);
			overflow: hidden;
			& > div {
				height: 140px;
				width: 40px;
				background-color: var(--green);
				position: absolute;
				bottom: 0px;
				left: 120px;
				box-shadow:
					80px -40px 0 0 var(--green),
					160px -110px 0 0 var(--green),
					160px 70px 0 0 var(--green),
					-80px -110px 0 0 var(--green),
					-80px 70px 0 0 var(--green);
			}
		}
	}
</style>

