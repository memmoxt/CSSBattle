<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f3ead2;
		--red: #d97d71;
		--purple: #857495;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			bottom: 65px;
			height: 170px;
			width: 360px;
			background-color: var(--red);
			&:before {
				position: absolute;
				content: '';
				height: 40px;
				width: 360px;
				background-color: var(--purple);
			}
			&:after {
				position: absolute;
				content: '';
				height: 140px;
				width: 30px;
				background-color: var(--purple);
				box-shadow: 330px 0 0 0 var(--purple);
			}
		}
	}
</style>

