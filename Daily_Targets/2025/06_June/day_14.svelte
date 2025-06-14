<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #6592cf;
		--yellow: #f7cb71;
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
			position: absolute;
			height: 180px;
			width: 220px;
			background-color: var(--yellow);
			clip-path: polygon(
				0 0,
				20px 0,
				20px 160px,
				200px 160px,
				200px 20px,
				60px 20px,
				60px 120px,
				160px 120px,
				160px 60px,
				100px 60px,
				100px 80px,
				140px 80px,
				140px 100px,
				80px 100px,
				80px 40px,
				180px 40px,
				180px 140px,
				40px 140px,
				40px 0px,
				220px 0px,
				220px 180px,
				0px 180px
			);
		}
	}
</style>

