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
		box-sizing: border-box;
		--green: #4a9a86;
		--yellow: #fae29e;
        background-color: var(--green);
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
			width: 80px;
			border: var(--yellow) solid 10px;
			translate: -150px;
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				border-radius: 50%;
				translate: 15px 55px;
			}
		}
		& > div:nth-child(2) {
			translate: 50px;
		}
		& > div:nth-child(3) {
			transform: rotate(180deg) translate(-100px);
		}
		& > div:nth-child(4) {
			transform: rotate(180deg) translate(-300px);
		}
	}
</style>
