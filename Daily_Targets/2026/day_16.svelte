<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--darkgreen: #0f3a22;
		--green: #289c5b;
		--white: #fbfae2;
        background-color: var(--darkgreen);
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
			height: 60px;
			width: 210px;
			background-color: var(--green);
			translate: 0px -60px;
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 60px;
				background-color: var(--white);
				translate: 0 120px;
				box-shadow:
					75px 0px var(--white),
					150px 0 var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				background-color: var(--darkgreen);
				border-radius: 50%;
				translate: 55px 40px;
			}
		}
	}
</style>

