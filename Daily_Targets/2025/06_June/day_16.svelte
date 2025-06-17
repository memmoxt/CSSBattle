<div class="main">
	<div>
		<div></div>
		<div></div>
	</div>
	<div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #d95362;
		--white: #d9d9d9;
        background-color: var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1) {
			position: absolute;
			top: 28px;
			height: 164px;
			width: 328px;
			/* background-color: black; */
			& > div {
				position: absolute;
				height: 164px;
				aspect-ratio: 1;
				background-color: var(--white);
				box-shadow: 164px 0 var(--red);
				&:before {
					content: '';
					position: absolute;
					height: 90px;
					aspect-ratio: 1;
					border-radius: 50%;
					translate: 36px 36px;
					background-color: var(--red);
					box-shadow: 165px 0 var(--white);
				}
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 90px;
			width: 328px;
			bottom: 18px;

			& > div {
				border-top: 80px solid var(--white);
				border-right: 164px solid transparent;
				border-left: 164px solid transparent;
				border-bottom: 0px solid transparent;
			}
		}
	}
</style>

