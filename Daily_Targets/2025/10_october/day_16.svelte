<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #b67024;
		--brown: #3b240c;
        background-color:var(--orange);
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
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--orange);
			border-radius: 50%;
			translate: -50px -50px;
			box-shadow: 0 0 0 30px var(--brown);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 150px;
				translate: -0px -50px;
				background-color: var(--orange);
				box-shadow: -100px 0 var(--brown);
			}
			&:after {
				content: '';
				position: absolute;
				height: 30px;
				width: 50px;
				background-color: var(--brown);
				translate: 50px 50px;
			}
		}
	}
</style>
