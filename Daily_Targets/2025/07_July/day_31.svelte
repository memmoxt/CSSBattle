<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #23384b;
		--yellow: #f0cd48;
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
			height: 155px;
			width: 50px;
			background-color: var(--yellow);
			translate: -65px -53px;
			border-top-left-radius: 25px;
			border-top-right-radius: 25px;
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 180px;
				background-color: var(--yellow);
				translate: 0px 105px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 260px;
				width: 50px;
				background-color: var(--yellow);
				translate: 130px 0px;
				border-radius: 25px/25px;
			}
		}
	}
</style>
