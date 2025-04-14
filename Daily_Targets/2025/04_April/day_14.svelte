<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #343400;
		--blue: #469dba;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--black);

		& > div {
			height: 160px;
			width: 250px;
			background-color: var(--blue);
			border-radius: 50%;

			/* opacity:0.5; */
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--blue);
				transform: translate(15px, 90px);
			}

			&:after {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--black);
				transform: translate(39px, 64px);
				box-shadow:
					70px 0 var(--black),
					140px 0 var(--black);
				border-radius: 50%;
			}
		}
	}
</style>

