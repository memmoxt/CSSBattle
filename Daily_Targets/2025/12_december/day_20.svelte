<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #1c204e;
		--orange: #e7772f;
		--white: #fef7f5;
        background-color: var(--blue);
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
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--white);
			border-radius: 50%;
			box-shadow: 0 0 0 30px var(--orange);
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 20px;
				translate: 20px 40px;
                box-shadow: 80px 0 var(--blue);
				background-color: var(--blue);
			}
		}
	}
</style>
