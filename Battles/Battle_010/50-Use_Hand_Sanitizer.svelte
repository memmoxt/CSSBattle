<div class="main">
	<div class="shaft"></div>
	<div class="shaft-base"></div>
	<div class="bottle-top"></div>
	<div class="bottle"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f3ac3c;
		--mustard: #998235;
		--green: #1a4341;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: var(--green);
		& > .shaft {
			height: 20px;
			width: 150px;
			border-radius: 20px;
			transform: translate(25px, 0px);
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 20px;
				border-radius: 20px;
				transform: translate(130px, 0);
				background-color: var(--yellow);
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				width: 20px;
				border-radius: 20px;
				transform: translate(130px, 50px);
				box-shadow: 0px 30px var(--mustard);
				background-color: var(--mustard);
			}
		}
		& > .shaft-base {
			width: 20px;
			height: 20px;
			background-color: var(--yellow);
		}
		& > .bottle-top {
			height: 20px;
			width: 50px;
			border-radius: 10px 10px 0 0;
			background-color: var(--yellow);
		}
		& > .bottle {
			height: 140px;
			width: 100px;
			border-radius: 20px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--yellow);
				box-shadow: -50px 0px 0 var(--mustard);
				transform: translate(50px, 30px);
				z-index: 2;
			}
			&:after {
				content: '';
				position: absolute;
				height: 85px;
				width: 100px;
				transform: translate(0px, 55px);
				background-color: var(--mustard);
				border-radius: 0 0 20px 20px;
				z-index: 1;
			}
		}
	}
</style>
