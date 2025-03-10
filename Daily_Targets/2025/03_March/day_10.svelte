<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--orange: #f58220;
		--white: #ffffff;
        background-color:var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 300px;
			width: 400px;
			background-color: var(--white);
			clip-path: polygon(
				139.5px 70px,
				199.5px 70px,
				173.5px 140px,
				233.5px 140px,
				259.5px 70px,
				319.5px 70px,
				259.5px 230px,
				199.5px 230px,
				226px 160px,
				166px 160px,
				139.5px 230px,
				79.5px 230px
			);
		}
	}
</style>

