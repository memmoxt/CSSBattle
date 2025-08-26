<div class="main">
	<div class="back"></div>
	<div class="front"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f0cd48;
		--dark: #243d83;
		--light: #6592cf;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
	}
	.back {
		height: 120px;
		width: 200px;
		background-color: var(--dark);
		position: absolute;
		&:before,
		&:after {
			content: '';
			position: absolute;
			height: 60px;
			width: 240px;
			background-color: var(--dark);
			border-radius: 20px/20px;
			transform: rotate(30deg);
			translate: -20px 30px;
		}
		&:after {
			transform: rotate(-30deg);
		}
	}
	.front {
		position: absolute;
		height: 60px;
		width: 100px;
		background-color: var(--light);
		&:before,
		&:after {
			content: '';
			position: absolute;
			height: 30px;
			width: 120px;
			background-color: var(--light);
			transform: rotate(30deg);
			translate: -10px 15px;
			border-radius: 10px;
		}
		&:after {
			transform: rotate(-30deg);
		}
	}
</style>
