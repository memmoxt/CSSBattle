<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #2d3464;
		--light-blue: #5aa4b7;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color: var(--blue);
		& > div {
			position: relative;
			align-self: start;
			height: 240px;
			width: 160px;
			display: grid;
			& > div {
				position: relative;
				height: 80px;
				width: 160px;
				background-color: var(--light-blue);
				border-bottom-right-radius: 80px;
				border-bottom-left-radius: 80px;
				/* opacity: 0.5; */
			}
			& > div:nth-child(3) {
				transform: rotate(180deg);
			}
		}
	}
</style>
