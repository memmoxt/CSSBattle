<div class="main">
	<div class=""></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fae29e;
		--green: #4a9a86;
		--gray: #4c4c6b;
        background-color:var(--yellow);
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
			position: absolute;
			height: 40px;
			width: 250px;
			background-color: var(--green);
			box-shadow: 0px 80px var(--gray);
			transform: translate(0px, -40px);
			&:before {
				position: absolute;
				content: '';
				height: 80px;
				width: 40px;
				background-color: var(--green);
				transform: translate(0px, -50px);
				box-shadow:
					210px 0 var(--green),
					210px 140px var(--gray),
					0px 140px var(--gray);
			}
		}
	}
</style>
