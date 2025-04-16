<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #4fc1ad;
		--black: #4c455b;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--green);

		& > div {
			position: absolute;
			height: 120px;
			width: 280px;
			background-color: var(--green);
			/* opacity: 0.5; */
			box-shadow: 0 0 0 40px var(--black);

			&:before {
				content: '';
				position: absolute;
				height: 220px;
				width: 40px;
				background-color: var(--black);
				transform: translate(40px, -91px);
				box-shadow: 160px 0 var(--black);
			}

			&:after {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--green);
				transform: translate(40px, -40px);
				box-shadow: 160px 0 var(--green);
			}
		}
	}
</style>
