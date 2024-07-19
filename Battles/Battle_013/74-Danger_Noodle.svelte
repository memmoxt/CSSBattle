<div class="main">
	<div class="half-circle"><div class="circle"></div></div>
	<div class="short-trail"></div>
	<div class="half-circle"><div class="circle"></div></div>
	<div class="long-trail"></div>
	<div class="half-circle"><div class="circle"></div></div>
	<div class="long-trail"></div>
	<div class="half-circle"><div class="circle"></div></div>
	<div class="long-trail"></div>
	<div class="half-circle"><div class="circle"></div></div>
	<div class="short-trail"></div>
	<div class="half-circle"><div class="circle"></div></div>
	<div class="short-trail"></div>
	<div class="head"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #191919;
		--orange: #e08027;
		background: var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > .half-circle {
			position: absolute;
			height: 35px;
			width: 70px;
			display: flex;
			justify-content: center;
			overflow: hidden;
			& > .circle {
				height: 30px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translateY(20px);
				background-color: var(--black);
				box-shadow:
					0 0 0 5px var(--orange),
					0 0 0 15px var(--black),
					0 0 0 20px var(--orange);
			}
		}
		& > .long-trail,
		& > .short-trail {
			position: absolute;
			width: 10px;
			background-color: var(--black);
			box-shadow: 0 0 0 5px var(--orange);
		}
		& > .long-trail {
			height: 150px;
			clip-path: polygon(-5px 0px, 15px 0px, 15px 150px, -5px 150px);
		}
		& > .short-trail {
			height: 50px;
			clip-path: polygon(-6px 0px, 15px 0px, 15px 50px, -6px 50px);
		}
		& > .head {
			position: absolute;
			height: 30px;
			width: 50px;
			background-color: var(--orange);
			transform: translate(90px, 0px);
			border-radius: 32px 50px 50px 32px;
			&:before {
				content: '';
				position: absolute;
				height: 10px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(30px, 2px);
				box-shadow: 0 16px 0 0 var(--black);
				background-color: var(--black);
			}
		}

		& > div:nth-child(1) {
			transform-origin: center;
			transform: rotate(180deg) translate(200px, 7.5px);
		}
		& > div:nth-child(2) {
			transform: translate(-175px, -50px);
		}
		& > div:nth-child(3) {
			transform: translate(-150px, -92px);
		}
		& > div:nth-child(4) {
			transform: translate(-125px, -0px);
		}
		& > div:nth-child(5) {
			transform: rotate(180deg) translate(100px, -92px);
		}
		& > div:nth-child(6) {
			transform: translate(-75px, 0px);
		}
		& > div:nth-child(7) {
			transform: translate(-50px, -93px);
		}
		& > div:nth-child(8) {
			transform: translate(-25px, 0px);
		}
		& > div:nth-child(9) {
			transform: rotate(180deg) translate(0px, -92px);
		}
		& > div:nth-child(10) {
			transform: translate(25px, 50px);
		}
		& > div:nth-child(11) {
			transform: translate(50px, 8px);
			clip-path: polygon(-5px 0px, 35px 0px, 35px 35px, -0px 35px);
		}
		& > div:nth-child(12) {
			transform: translate(75px, 0px) rotate(90deg);
		}
	}
</style>
