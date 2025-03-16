<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #eac049;
		--green: #51a499;
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
			box-shadow: 0 0 0 20px var(--green);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--green);
				height: 40px;
				aspect-ratio: 1;
				transform: translate(-100%, -100%);
				box-shadow:
					180px 0 0 var(--green),
					180px 180px 0 var(--green),
					0px 180px 0 var(--green);
			}
		}
	}
</style>

