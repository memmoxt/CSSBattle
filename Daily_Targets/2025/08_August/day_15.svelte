<div class="main">
	<div></div>
	<div class="item"></div>
	<div class="item"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--white: #ffeff2;
		--blue: #4f77ff;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			height: 160px;
			width: 360px;
			background-color:var(--blue);
			border-top-left-radius: 100px;
			border-top-right-radius: 100px;
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 160px;
				background-color: var(--white);
				translate: 100px 30px;
			}
		}
		& > .item:nth-child(2) {
			height: 80px;
			width: 50px;
			background-color: var(--blue);
			position: absolute;
			translate: -45px 0;
			border-top-left-radius: 50px;
		}
		& > .item:nth-child(3) {
			height: 80px;
			width: 50px;
			background-color: var(--blue);
			position: absolute;
			border-top-right-radius: 50px;
			translate: 45px 0;
		}
	}
</style>
