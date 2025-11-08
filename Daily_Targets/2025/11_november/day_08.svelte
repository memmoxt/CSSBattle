<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #ffe5ac;
		--black: #313131;
        background-color: var(--yellow);
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
			height: 50px;
			width: 120px;
			translate: 0px -40px;
			box-shadow: 0px 80px var(--black);
			background-color: var(--black);
			border-radius: 50px / 50px;
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 50px;
				background-color: var(--yellow);
				translate: -0px 10px;
				border-radius: 50px / 50px;
                border-bottom-left-radius:0px;
                border-bottom-right-radius:0px;
				box-shadow: 70px 0px var(--yellow);
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--black);
				translate: 10px 20px;
				border-radius: 50%;
				box-shadow: 70px 0 var(--black);
			}
		}
	}
</style>
