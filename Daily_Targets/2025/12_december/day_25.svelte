<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #1bbc63;
		--darkgreen: #0f6b38;
		--darkblue: #11092d;
		--yellow: #ffca00;
        background-color:var(--darkblue);
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
			height: 20px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			translate: 0 -80px;
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				width: 50px;
				background-color: var(--green);
				translate: -15px 40px;
				box-shadow:
					-15px 40px var(--darkgreen),
					15px 40px var(--darkgreen);
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				width: 110px;
				background-color: var(--green);
				translate: -45px 120px;
				box-shadow:
					-15px 40px var(--darkgreen),
					15px 40px var(--darkgreen);
			}
		}
	}
</style>
