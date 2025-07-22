<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--gray: #423f36;
		--slate: #bbbbbb;
		--red: #ec2f28;
        background-color: var(--gray);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 50px;
			width: 50px;
			background-color: var(--slate);
			translate: 0px -95px;
			border-radius: 50%;
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				width: 80px;
				background-color: var(--red);
				translate: -15px 170px;
				border-bottom-left-radius: 10px;
				border-bottom-right-radius: 10px;
			}
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				width: 100px;
				background-color: var(--gray);
				translate: -25px 40px;
				border-radius: 20px/20px;
				box-shadow:
					0px 0px 0 10px var(--slate),
					0 0 0 20px var(--gray);
			}
		}
	}
</style>
