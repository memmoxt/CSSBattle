<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--pink: #dc9da6;
		--brown: #6e3c3c;
        background-color:var(--pink);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div:nth-child(1) {
			height: 20px;
			width: 200px;
			background-color: var(--brown);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--brown);
				height: 200px;
				width: 20px;
				translate: 90px -90px;
			}
			&:after {
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--pink);
				border-radius: 50%;
				box-shadow: 0 0 0 30px var(--brown);
				translate: 80px -10px;
				content: '';
			}
		}
		& > div:nth-child(2) {
			position: absolute;
			height: 20px;
			width: 200px;
			background-color: var(--brown);
			transform: rotate(-45deg);
		}
	}
</style>
