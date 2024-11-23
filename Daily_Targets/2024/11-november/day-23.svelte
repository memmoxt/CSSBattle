<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #eeb850;
		--blue: #243d83;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 110px;
			width: 220px;
			background-color: var(--blue);
			border-radius: 20px/20px;
			&:before {
				content: '';
				position: absolute;
				height: 15px;
				width: 70px;
				background-color: var(--yellow);
                transform:translate(75px,20px);
                box-shadow:0 55px var(--yellow);
			}
		}
	}
</style>

