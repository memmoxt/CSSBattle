<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #3f4869;
		--red: #e25c57;
		background-color: var(--purple);
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
			height: 100px;
			border-radius: 50%;
			translate: 0 150px;
			aspect-ratio: 1;
			position: absolute;
			background-color: var(--red);
			box-shadow:
				-80px -300px var(--red),
				80px -300px var(--red);
			&:before {
				content: '';
				position: absolute;
				height: 300px;
				width: 20px;
				translate: 40px -250px;
				background-color: var(--red);
				box-shadow:
					-80px 0px var(--red),
					80px 0px var(--red);
			}
		}
	}
</style>
