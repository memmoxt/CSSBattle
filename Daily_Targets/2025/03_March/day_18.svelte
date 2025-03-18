<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--teal: #51a499;
		--yellow: #eac049;
        background-color:var(--yellow);
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
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			/* opacity: 0.5; */
			box-shadow: 0 0 0 20px var(--teal);
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				background-color: var(--teal);
				box-shadow:
					200px 0 0 var(--teal),
					0px 200px 0 var(--teal),
					200px 200px 0 var(--teal);
				transform: translate(-60px, -60px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				box-shadow:
					200px 0 0 var(--yellow),
					0px 200px 0 var(--yellow),
					200px 200px 0 var(--yellow);
				transform: translate(-40px, -40px);
			}
		}
	}
</style>

