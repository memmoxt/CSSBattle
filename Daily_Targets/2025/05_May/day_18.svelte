<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--beige: #f3ead2;
		--black: #4c455b;
		--slate: #c0d6e7;
		--red: #d96c7b;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--beige);
		& > div:nth-child(1) {
			position: absolute;
			height: 50px;
			width: 150px;
			background-color: var(--red);
			transform: rotate(-45deg) translate(0px, 50px);
			&:after {
				content: '';
				position: absolute;
				height: 150px;
				width: 50px;
                transform:translate(-0px,-100px);
				background-color: var(--black);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			border-top: 70px solid var(--slate);
			border-right: 70px solid transparent;
			border-bottom: 70px solid transparent;
			border-left: 70px solid transparent;
			transform: translate(0px, 35px);
		}
	}
</style>
