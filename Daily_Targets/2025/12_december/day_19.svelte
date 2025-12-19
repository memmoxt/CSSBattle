<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #7e6293;
		--yellow: #e8ba79;
        background-color: var(--purple);
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
			height: 230px;
			width: 330px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 200px;
				background-color: var(--purple);
				translate: 20px 110px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				width: 250px;
				background-color: var(--purple);
				translate: 20px 60px;
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 40px;
			width: 270px;
			background-color: var(--purple);
			translate: -10px -95px;
			&:before {
				content: '';
				position: absolute;
				height: 170px;
				width: 40px;
				background-color: var(--purple);
				translate: 270px 40px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 130px;
				width: 30px;
				background-color: var(--purple);
                translate: 220px 80px;
			}
		}
	}
</style>
