<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #ffea9b;
		--green: #4a9a86;
        background-color: var(--yellow);
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
			height: 240px;
			width: 340px;
			background-color: var(--green);
			clip-path: polygon(
				0px 0px,
				100px 0px,
				100px 30px,
				130px 30px,
				130px 60px,
				210px 60px,
				210px 30px,
				240px 30px,
				240px 0px,
				100% 0px,
				100% 30px,
				310px 30px,
				310px 60px,
				280px 60px,
				280px 90px,
				185px 90px,
				185px 100%,
				155px 100%,
				155px 90px,
				60px 90px,
				60px 60px,
				30px 60px,
				30px 30px,
				0px 30px
			);
		}
	}
</style>
