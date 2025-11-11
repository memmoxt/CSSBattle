<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #050044;
		--red: #a4215d;
		--white: #f3ead2;
        background-color:var(--blue);
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
			height: 100px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--blue);
			translate: -0px -30px;
			box-shadow: 0 0 0 40px var(--white);
			&:before {
				content: '';
				position: absolute;
				translate: -80px -20px;
				height: 40px;
				width: 260px;
				background-color: var(--red);
				box-shadow:
					0px -30px var(--blue),
					-20px 160px var(--red),
					20px 160px var(--red);
			}
		}
	}
</style>
