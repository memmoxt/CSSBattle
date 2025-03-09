<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #c12e33;
		--black: #323130;
		background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 300px;
			width: 120px;
			background-color: var(--black);
			/* opacity: 0.5; */
			transform: translate(-60px);
			clip-path: polygon(
				0 0,
				40px 0px,
				120px 80px,
				40px 160px,
				40px 300px,
				0 300px,
				0 160px,
				80px 80px
			);
		}
		& > div:nth-child(2) {
			transform: translate(60px) scaleX(-1);
		}
	}
</style>

