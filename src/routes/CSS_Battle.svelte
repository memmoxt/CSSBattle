<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #3f4869;
		--green: #70b7a5;
        background-color: var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			height: 260px;
			width: 260px;
			background-color: var(--green);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--black);
				box-shadow:
					220px 0px var(--black),
					-5px 220px var(--black),
					215px 220px var(--black),
					220px 220px var(--black),
					110px 110px 0px 5px var(--black),
					43px 42px 0 22px var(--black),
					177px 42px 0 22px var(--black),
					177px 177px 0 22px var(--black),
					42px 177px 0 22px var(--black);
			}
			&:after {
				content: '';
				position: absolute;
				height: 150px;
				width: 20px;
				translate: 20px 5px;
				background-color: var(--black);
				box-shadow: 200px 10px var(--black);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 20px;
			width: 100px;
			translate: 0 99px;
			background-color: var(--black);
            box-shadow:0px -199px var(--black);
		}
	}
</style>
