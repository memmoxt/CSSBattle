<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #4763b1;
		--white: #d9d9d9;
        background-color: var(--blue);
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
			height: 30px;
			width: 40px;
			background-color: var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 60px;
				translate: -10px -135px;
				box-shadow: 0px 200px var(--white);
				background-color: var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 60px;
				width: 100px;
				background-color: var(--white);
				box-shadow: 300px 0px var(--white);
				translate: -180px -15px;
			}
		}
	}
</style>
