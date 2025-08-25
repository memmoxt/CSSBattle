<div class="main">
	<div class="stack"></div>
	<div class="stack"></div>
	<div class="stack"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #3a335a;
		--white: #ffffff;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > .stack {
			position: absolute;
			height: 170px;
			width: 140px;
			background-color: var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 140px;
				background-color: var(--purple);
				translate: 0px 30px;
				box-shadow: 0 70px var(--purple);
			}
		}
		& > .stack:nth-child(2) {
			transform: rotate(-15deg);
			translate: 170px;
		}
		& > .stack:nth-child(3) {
			transform: rotate(15deg);
			translate: -170px;
		}
	}
</style>
