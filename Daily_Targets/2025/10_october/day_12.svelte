<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #4763b1;
		--white: #ffffff;
        background-color: var(--blue);
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
			height: 118px;
			aspect-ratio: 1;
			background-color: var(--blue);
			display: grid;
			grid-template-columns: repeat(2, 1fr);
			grid-template-rows: repeat(2, 1fr);
			gap: 18px;
			& > div {
				position: relative;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--white);
			}
			& > div:nth-child(1) {
				position: absolute;
				height: 40px;
				translate: 39px 39px;
				background-color: var(--blue);
				aspect-ratio: 1;
				border-radius: 50%;
				z-index: 2;
			}
		}
	}
</style>
