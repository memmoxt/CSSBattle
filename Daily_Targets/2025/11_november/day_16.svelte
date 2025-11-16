<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #8cfadc;
		--dark: #1a4341;
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
			height: 120px;
			aspect-ratio: 1;
			border-radius: 50%;
			transform: translate(-20px, 8px);
			box-shadow: 38px 0px var(--dark);
			background-color: var(--dark);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				translate: 55px -4px;
                box-shadow: -14px -14px 0 30px var(--blue);
				transform: rotate(45deg);
				background-color: var(--dark);
			}
		}
	}
</style>
