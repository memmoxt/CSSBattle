<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #085328;
		--light: #8cb457;
		background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 240px;
			width: 300px;
			background-color: var(--light);
			&:before {
				content: '';
				position: absolute;
				height: 180px;
				aspect-ratio: 1;
				background-color: var(--green);
				translate: 60px 30px;
				box-shadow:
					-210px 0 var(--green),
					210px 0 var(--green);
			}
		}
	}
</style>
