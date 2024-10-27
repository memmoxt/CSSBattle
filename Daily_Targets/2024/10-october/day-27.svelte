<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #eca03d;
		--black: #191210;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--black);
		& > div {
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				width: 80px;
				border-radius: 50px/50px;
				top: 110px;
				left: 160px;
				background-color: var(--black);
				box-shadow:
					-65px -80px 0 0 var(--black),
					-0px -80px 0 0 var(--black),
					65px -80px 0 0 var(--black),
					-65px 0 0 0 var(--black),
					65px 0 0 0 var(--black),
					-65px 80px 0 0 var(--black),
					0 80px 0 0 var(--black),
					65px 80px 0 0 var(--black);
			}
		}
	}
</style>

