<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--amber: #d27644;
		--black: #000000;
		--white: #fef6e2;
        background-color: var(--amber);
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
			height: 150px;
			aspect-ratio: 1;
			position: absolute;
			background-color: var(--black);
			border-radius: 50%;
			translate: 0px 15px;

			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 150px;
				background-color: var(--black);
				translate: 0px 80px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				width: 120px;
				translate: 15px 150px;
				background-color: var(--amber);
				box-shadow:
					30px 30px var(--black),
					-30px 30px var(--black);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 20px;
			aspect-ratio: 1;
			background-color: white;
			translate: 0px 10px;
			border-radius: 50%;
		}
	}
</style>
