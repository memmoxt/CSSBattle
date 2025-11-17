<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fef7f5;
		--blue: #555fd9;
        background-color:var(--white);
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
			height: 240px;
			width: 340px;
			background-color: var(--blue);
			clip-path: polygon(
				0 0,
				100% 0px,
				100% 60px,
				70px 60px,
				70px 80px,
				308px 80px,
				308px 160px,
				71px 160px,
				71px 180px,
				340px 180px,
				340px 240px,
				0px 240px,
				0px 220px,
				320px 220px,
				320px 200px,
				50px 200px,
				50px 140px,
				290px 140px,
				290px 100px,
				50px 100px,
				50px 40px,
				320px 40px,
				320px 20px,
				0px 20px
			);
		}
	}
</style>
