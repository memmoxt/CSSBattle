<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #49c85b;
		--blue: #2f5a76;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			background-color: var(--blue);
			height: 220px;
			width: 160px;
			clip-path: polygon(
				80px 0,
				128px 82.5px,
				159px 82.5px,
				143.5px 110px,
				159px 136px,
				128px 136px,
				80px 219.0px,
                32px 136.0px,
                1px 136.0px,
                17px 110.0px,
                1px 82.5px,
                32px 82.5px
			);
		}
	}
</style>

