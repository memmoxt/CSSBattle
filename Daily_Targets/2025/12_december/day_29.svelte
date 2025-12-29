<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #e38f66;
		--white: #fffbda;
        background-color:var(--orange);
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
			background-color: var(--white);
			translate: -50px 30px;
			box-shadow: 100px -60px var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--orange);
                translate:50px -30px;
                border-top-right-radius:50px;
                border-bottom-left-radius:50px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--white);
				transform: translate(80px);
			}
		}
	}
</style>
