<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		--white: #f9ddc6;
		--purple: #594c94;
        background-color:var(--white);

		& > div {
			position: absolute;
			top: 45px;
			background-color: var(--purple);
			height: 88px;
			width: 268px;
			clip-path: polygon(70px 0, 197px 0, 267px 88px, 0 88px);
		}
		& > div:nth-child(1) {
			&:before {
				content: '';
				position: absolute;
				height: 90px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--white);
				transform: translate(89px, 43px);
			}
		}
		& > div:nth-child(2) {
			top: 166px;
			transform: scaleY(-1);
		}
	}
</style>

