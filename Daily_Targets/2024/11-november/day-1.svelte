<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #515697;
		--orange: #e38f66;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: end;
        background-color:var(--blue);
		& > div {
			height: 288px;
			width: 360px;
			background-color: var(--orange);
            border-top-left-radius: 180px;
            border-top-right-radius: 180px;
			&:before {
				content: '';
				position: absolute;
				height: 71px;
				width: 35px;
				background-color: var(--blue);
				left: 56px;
				bottom: 0px;
				box-shadow:
					73px 0 0 0 var(--blue),
					180px 0 0 0 var(--blue),
					252px 0 0 0 var(--blue);
			}
		}
	}
</style>

