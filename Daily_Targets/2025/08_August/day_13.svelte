<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		--green: #5a9f48;
		--black: #23384b;
		background-color: var(--green);
		& > div {
			height: 120px;
			aspect-ratio: 1;
			background-color: var(--green);
			border-radius: 50%;
			translate: 0 -40px;
			box-shadow: 0 0 0 20px var(--black);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--green);
				border-radius: 10px;
				height: 120px;
				width: 180px;
				translate: -30px 80px;
				box-shadow: 0 0 0 20px var(--black);
			}
			&:after {
				content: '';
				position: absolute;
				height: 80px;
				width: 40px;
				background-color: var(--green);
				translate: 40px 140px;
				box-shadow: 0 0 0 20px var(--black);
				clip-path: polygon(-20px -20px, 150px -20px, 150px 80px, -20px 80px);
			}
		}
	}
</style>
