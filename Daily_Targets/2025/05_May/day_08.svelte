<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #0a4756;
		--lightgreen: #5a9f48;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--green);
		& > div {
			position: absolute;
			height: 240px;
			aspect-ratio: 1;
			background-color: var(--lightgreen);
			border-radius: 50%;
			&:before {
				position: absolute;
				content: '';
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--green);
				transform: translate(60px, 60px);
			}
			&:after {
				position: absolute;
				content: '';
				height: 100px;
				aspect-ratio: 1;
				border-radius: 50%;
				transform: translate(70px, 70px);
				background-color: var(--lightgreen);
			}
		}
	}
</style>

