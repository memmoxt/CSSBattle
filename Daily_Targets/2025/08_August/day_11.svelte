<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--pink: #b673a6;
		--blue: #619ebf;
		--white: #d9d9d9;
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
			height: 100%;
			width: 100%;
			background-color: var(--pink);
			&:before {
				content: '';
				position: absolute;
				height: 150px;
				aspect-ratio: 1;
				background-color: var(--blue);
				translate: -30px 180px;
				border-top-right-radius: 10px;
				border-top-left-radius: 10px;
				box-shadow:
					310px 0 var(--blue),
					0 0 0 30px var(--white),
					310px 0 0 30px var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--white);
				translate: 180px 130px;
				border-radius: 50%;
				box-shadow:
					80px 30px var(--blue),
					-80px 30px var(--blue);
			}
		}
	}
</style>
