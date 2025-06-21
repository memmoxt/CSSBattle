<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #6592cf;
		--yellow: #f7cb71;
		--white: #fefeff;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: start;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 80px;
			width: 200px;
			transform: translate(150px);
			background-color: var(--yellow);
			&:before {
				position: absolute;
				content: '';
				height: 113px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				transform: translate(-27px, -17px) rotate(45deg);
                box-shadow:114px -114px 0 0 var(--blue);
			}
			&:after {
				position: absolute;
				content: '';
				height: 28px;
				aspect-ratio: 1;
				transform: translate(-24px, 26px) rotate(45deg);
				background-color: var(--white);
			}
		}
	}
</style>
