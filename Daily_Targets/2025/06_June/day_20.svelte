<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #fefeff;
		--blue: #6592cf;
		--yellow: #eeb850;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: start;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			position: relative;
			height: 220px;
			width: 320px;
			background-color: var(--blue);
			align-self: start;
			transform: translate(20px, 20px);
            overflow: hidden;
			&::before {
				content: '';
				position: absolute;
				height: 100px;
				width: 260px;
				background-color: var(--white);
				box-shadow: 0 160px 0 0px var(--white);
				transform: translate(60px);
			}
		}
	}
</style>
