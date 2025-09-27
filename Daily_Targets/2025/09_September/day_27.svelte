<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #eddf5a;
		--red: #e8625e;
		--black: #323232;
        background-color:var(--yellow);
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
			height: 60px;
			width: 260px;
			translate: 0 -30px;
			--brickcolor: var(--red);
			background-color: var(--brickcolor);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 60px;
				background-color: var(--brickcolor);
				translate: 30px -40px;
				box-shadow: 140px 0 var(--brickcolor);
			}
		}
		& > div:nth-child(2) {
			transform: rotate(-180deg) translateY(-60px);
			--brickcolor: var(--black);
		}
	}
</style>
