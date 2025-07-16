<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #32295a;
		--green: #48bf7d;
		background-color: var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 200px;
			width: 200px;
			background-color: var(--purple);
			border-radius: 50%;
			translate: 0px -40px;
			box-shadow: 0px 40px 0 50px var(--green);

			&:before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--purple);
				translate: 75px 100px;
				border-radius: 100%;
				box-shadow: 0 15px 0 25px var(--green);
			}
		}
	}
</style>
