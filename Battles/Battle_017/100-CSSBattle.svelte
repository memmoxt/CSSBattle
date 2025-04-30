<div class="main">
	<div class="base"></div>
	<div class="box"></div>
	<div class="sword"></div>
	<div class="sword-2"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #14313e;
		--yellow: #ffdf00;
        background-color: var(--green);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > .base {
			height: 150px;
			width: 274px;
			background-color: var(--yellow);
			border-radius: 20px;
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 294px;
				background-color: var(--yellow);
				transform: translate(-10px, 55px);
				border-radius: 5px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 224px;
				transform: translate(25px, 25px);
				border-radius: 10px;
				background-color: var(--green);
			}
		}
		& > .box {
			position: absolute;
			height: 150px;
			width: 194px;
			background-color: var(--green);
		}
		& > .sword,
		& > .sword-2 {
			position: absolute;
			height: 210px;
			width: 20px;
			background-color: var(--yellow);
			transform-origin: center;
			transform: rotate(45deg) translateX(-4px) translateY(-2px);
			box-shadow: 0 0 0 15px var(--green);
			clip-path: polygon(
				-5px 14px,
				10px -1px,
				25px 14px,
				50px 150px,
				25px 150px,
				50px 150px,
				50px 170px,
				20px 170px,
				20px 218px,
				0px 218px,
				0px 170px,
				-30px 170px,
				-30px 150px,
				-5px 150px,
				-50px 150px
			);
			border-radius: 8px;
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				width: 30px;
				transform: translateX(-5px) translateY(0px);
				background-color: var(--yellow);
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				width: 80px;
				transform: translateX(-30px) translateY(150px);
				background-color: var(--yellow);
			}
		}
		& > .sword-2 {
			transform: rotate(-45deg) translateX(4px) translateY(-2px);
		}
	}
</style>
