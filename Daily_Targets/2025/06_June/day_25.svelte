<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark-purple: #5e2bb7;
		--blue: #b6ebe7;
		--light-purple: #9382e4;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 160px;
			aspect-ratio: 1;
			background-color: var(--light-purple);
			position: relative;
            overflow: hidden;
            border-bottom-left-radius: 80px;
			&::before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--dark-purple);
				translate: 120px;
			}
			&::after {
				content: '';
				position: absolute;
				height: 80px;
				aspect-ratio: 1;
				translate: 0px 80px;
				background-color: var(--dark-purple);
			}
		}
	}
</style>
