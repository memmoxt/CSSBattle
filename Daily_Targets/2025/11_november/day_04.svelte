<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #000000;
		--green: #00d47e;
		background-color: var(--green);
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
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--green);
			box-shadow:
				0 0 0 25px var(--black),
				130px 0 var(--green),
				130px 0 0 25px var(--black),
				-130px 0 var(--green),
				-130px 0 0 25px var(--black);
			&:before {
				content: '';
				position: absolute;
				height: 16px;
				width: 40px;
				translate: 5px 17px;
				background-color: var(--black);
				box-shadow:
					150px 0 var(--black),
					-150px 0 var(--black);
			}
		}
	}
</style>
