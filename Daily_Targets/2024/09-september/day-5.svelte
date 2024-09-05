<div class="main">
	<div class="four-boxes">
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
	<div class="four-boxes">
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #9076d8;
		--white: #f3ead2;
		background-color: var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		align-content: flex-start;
		gap: 14px;
		& > .four-boxes {
			height: 94px;
			width: 224px;
			transform: translateY(1px);
			display: flex;
			column-gap: 16px;
			& > div {
				background-color: var(--white);
				width: 44px;
				align-self: end;
			}
			& > div:nth-child(1) {
				height: 94px;
			}
			& > div:nth-child(2) {
				height: 64px;
			}
			& > div:nth-child(3) {
				height: 43px;
			}
			& > div:nth-child(4) {
				height: 28px;
			}
		}

		& > .four-boxes:nth-child(2) {
			& > div:nth-child(1) {
				height: 93px;
			}
			& > div:nth-child(2) {
				height: 63px;
			}
			& > div:nth-child(3) {
				height: 42px;
			}
			& > div:nth-child(4) {
				height: 27px;
			}
			transform: scaleY(-1);
		}
	}
</style>
