<div class="main">
	<div class="fox">
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #edaf38;
		--white: #ffffcd;
		background: var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > .fox {
			height: 190px;
			width: 140px;
			background-color: var(--white);
			clip-path: polygon(0px 50px, 50% 100%, 100% 50px, 115px 0, 90px 50px, 50px 50px, 25px 0);
			& > div {
				position: absolute;
				height: 30px;
				width: 30px;
				transform: translate(35px, 75px);
				background-color: var(--yellow);
				clip-path: polygon(0px 0px, 100% 0, 50% 100%);
			}
			& > div:nth-child(2) {
				transform: translate(76px, 75px);
			}
		}
	}
</style>


