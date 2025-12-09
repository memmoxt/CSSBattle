<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #668884;
		--white: #eed9d9;
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
			height: 10px;
			width: 50px;
			background-color: var(--white);
			box-shadow:
				-110px 0px var(--white),
				110px 0px var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				translate: -160px -15px;
				box-shadow:
					110px 0px var(--white),
					220px 0px var(--white),
					330px 0 var(--white);
			}
		}
	}
</style>
