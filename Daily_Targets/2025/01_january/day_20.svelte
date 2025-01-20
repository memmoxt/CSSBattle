<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--purple: #594c94;
		--white: #f9ddc6;
		background-color: var(--purple);
		& > div {
			position: absolute;
			top: 11px;
			height: 50px;
			width: 220px;
			background-color: var(--white);
			&:before {
				position: absolute;
				content: '';
				right: 0px;
				top: 50px;
				background-color: var(--white);
				width: 26px;
				height: 26px;
			}
		}
		& > div:nth-child(2) {
			top: 87px;
			transform: scaleX(-1);
		}
		& > div:nth-child(3) {
			top: 163px;
		}
		& > div:nth-child(4) {
			top: 239px;
			&:before {
				height: 0px;
			}
		}
	}
</style>
