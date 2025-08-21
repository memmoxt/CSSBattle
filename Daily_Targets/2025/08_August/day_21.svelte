<div class="main">
	<div class="head"></div>
	<div class="neck"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--dark: #526766;
		--light: #b9c99f;
		background-color: var(--light);
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
	div {
		position: absolute;
	}
	.head {
		top: 0px;
		height: 150px;
		width: 300px;
		background-color: var(--dark);
		overflow: hidden;
		&:before {
			content: '';
			position: absolute;
			height: 50px;
			aspect-ratio: 1;
			background-color: var(--light);
			border-radius: 50%;
			translate: 75px 50px;
			box-shadow: 100px 0 0 var(--light);
		}
		&:after {
			content: '';
			position: absolute;
			height: 50px;
			width: 100px;
			background-color: var(--light);
			translate: 0 50px;
			box-shadow: 200px 0 var(--light);
		}
	}
	.neck {
		height: 50px;
		width: 50px;
		background-color: var(--dark);
		translate: 0 25px;
		box-shadow:
			-175px -100px var(--dark),
			175px -100px var(--dark);
		&:before {
			content: '';
			position: absolute;
			height: 100px;
			width: 400px;
			bottom: -100px;
			translate: -175px 0px;
			background-color: var(--dark);
		}
	}
</style>
