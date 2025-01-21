<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--green: #2f5a76;
		--light: #bfe33a;
        background-color:var(--green);
		& > div {
			height: 140px;
			width: 384px;
			background-color: var(--light);
			&:before {
				position: absolute;
				content: '';
				height: 70px;
				aspect-ratio: 1;
				background-color: var(--light);
				top: 115px;
				left: 165px;
				transform: rotate(45deg);
                box-shadow:0 0 0 40px var(--green);
			}
		}
	}
</style>

