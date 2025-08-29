<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--beige: #f1e1be;
		--brown: #7c7565;
        background-color:var(--brown);
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
			height: 90px;
			aspect-ratio: 1;
			background-color: var(--brown);
			box-shadow:
				-10px 0 0 75px var(--beige),
				10px 0 0 75px var(--beige);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 200px;
				background-color: var(--beige);
				translate: -155px 165px;
				box-shadow: 200px -270px var(--beige);
			}
		}
	}
</style>
