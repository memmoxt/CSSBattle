<div class="main">
	<div class="eyes"></div>
	<div class="mouth">
		<div class="mouth-topPart"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #293462;
		--red: #fe5f55;
		--brown: #a64942;
		--white: #fff1c1;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background: var(--blue);
		& > .eyes,
		& > .eyes:after {
			height: 10px;
			aspect-ratio: 1;
			border-radius: 50%;
			transform: translate(-35px, -40px);
			box-shadow:
				0 0 0 10px var(--white),
				0 0 0 20px var(--red),
				25px 55px 0 0px var(--blue);
			background-color: var(--blue);
			z-index: 1;
		}
		& > .eyes:after {
			content: '';
			position: absolute;
			transform: translate(70px, 0px) scaleX(-1);
		}
		& > .mouth {
			position: absolute;
			transform: translate(0, 10px);
			height: 100px;
			width: 150px;
			background-color: var(--brown);
			border-radius: 50px 50px 50px 50px;
			overflow: hidden;
			z-index: 0;
			& > .mouth-topPart {
				height: 100px;
				width: 150px;
				background-color: var(--red);
				clip-path: ellipse(105px 50px at 50% 20%);
			}
		}
	}
</style>
