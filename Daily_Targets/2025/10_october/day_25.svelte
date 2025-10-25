<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--beige: #e8ad6d;
		--brown: #3b240c;
        background-color: var(--beige);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		padding: 30px;
		grid-template-columns: 260px 50px;
		gap: 0px 30px;
		grid-template-rows: repeat(3, 1fr);
		& > div:nth-child(2n + 1) {
			position: relative;
			height: 15px;
			width: 260px;
			background-color: var(--brown);
		}
		& > div:nth-child(2n + 2) {
			position: relative;
			height: 15px;
			width: 50px;
			background-color: var(--brown);
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 15px;
				background-color: var(--brown);
				translate: 18px -18px;
			}
		}
	}
</style>
