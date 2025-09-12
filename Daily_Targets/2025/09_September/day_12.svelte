<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #d24444;
		--yellow: #f3da7a;
        background-color:var(--red);
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
			position: absolute;
			height: 230px;
			border-radius: 50%;
			box-shadow: 0 0 0 20px var(--yellow);
			aspect-ratio: 1;
			background-color: var(--red);
			display: flex;
			justify-content: center;
			align-items: center;
			& > div {
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				transform-origin: 0px 105px;
			}
			& > div:nth-child(1) {
				translate: 0px -105px;
			}
			& > div:nth-child(2) {
				translate: 10px -110px;
				transform: rotate(45deg);
			}
			& > div:nth-child(3) {
				translate: 20px -105px;
				transform: rotate(90deg);
			}
			& > div:nth-child(4) {
				translate: 25px -95px;
				transform: rotate(135deg);
			}
			& > div:nth-child(5) {
				translate: 0px 105px;
				transform: rotate(0deg);
			}
			& > div:nth-child(6) {
				translate: 10px -81px;
				transform: rotate(-135deg);
			}
			& > div:nth-child(7) {
				translate: 0px -85px;
				transform: rotate(-90deg);
			}
			& > div:nth-child(8) {
				translate: -4px -95px;
				transform: rotate(-45deg);
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 80px;
			width: 20px;
			translate: 0px -30px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				width: 80px;
				background-color: var(--yellow);
				translate: 0px 60px;
			}
		}
	}
</style>
