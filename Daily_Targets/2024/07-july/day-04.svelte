<div class="main">
	<div class="guide">
		<div class="circle"></div>
		<div class="circle"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffff;
		--blue: #4f77ff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--blue);
		& > .guide {
			height: 240px;
			width: 340px;
			display: flex;
			justify-self: space-between;
			align-items: space-between;
			& > .circle,
			& > .circle:before {
				height: 150px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--white);
			}
			& > .circle:before {
				content: '';
				position: absolute;
				transform: translate(40px, 40px);
				background-color: var(--blue);
			}
			& > .circle:nth-child(2) {
				transform: translate(40px, 90px);
			}
			& > .circle:nth-child(2):before {
				transform: translate(-40px, -40px);
			}
		}
	}
</style>
