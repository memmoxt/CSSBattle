<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #51a499;
		--dark: #23384b;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 220px;
			width: 80px;
			translate: -40px 10px;
			border-radius: 50px/50px;
			background-color: var(--dark);
			&::before {
				content: '';
				position: absolute;
				height: 140px;
				width: 80px;
				translate: 0px 40px;
				background-color: var(--green);
			}
			&::after {
				content: '';
				position: absolute;
				height: 140px;
				width: 80px;
				background-color: var(--dark);
				translate: 80px 40px;
			}
		}
	}
</style>
