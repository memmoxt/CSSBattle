<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--beige: #e8ad6d;
		--black: #000000;
		--white: #ffffff;
        background-color:var(--beige);
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
			height: 120px;
			aspect-ratio: 1;
			background-color: var(--beige);
			border-top-right-radius: 30px;
			border-bottom-left-radius: 30px;
			box-shadow: 0 0 0 40px var(--black);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--white);
                translate:-40px -40px;
                box-shadow: 160px 160px var(--white);
			}
		}
	}
</style>
