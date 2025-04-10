<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffff;
		--gray: #bdc8d1;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		background-color: var(--white);
		& > div {
			position: absolute;
			height: 140px;
			width: 100px;
			top: 52px;
			background-color: var(--gray);
			box-shadow:
				120px 0 var(--gray),
				-120px 0 var(--gray);
			/* opacity:0.5; */
			&:before {
				content: '';
				position: absolute;
				height: 35px;
				width: 340px;
				background-color: var(--gray);
				bottom: -55px;
				right: -120px;
			}
		}
	}
</style>
