<div class="main">
	<div class="box"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #191919;
		--blue: #5dbcf9;
	}

	.main {
		position: absolute;
		overflow: hidden;
		height: 300px;
		width: 400px;
		background-color: var(--blue);
		& > .box,
		& > .box:before {
			position: absolute;
			height: 110px;
			width: 140px;
			box-shadow:
				-150px 50px 0 var(--black),
				-150px -100px 0 var(--black),
				-150px 200px 0 var(--black),
				-0px 150px 0 var(--black),
				-0px -150px 0 var(--black);
			top: 70px;
			left: 55px;
			background-color: var(--black);
		}
		& > .box:before {
			content: '';
			position: absolute;
			transform: translate(245px, -70px);
		}
	}
</style>
