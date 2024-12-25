<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		--black: #3f4869;
		--yellow: #f4da64;
        background-color:var(--black);
		& > div {
			background-color: var(--yellow);
			/* opacity: 0.5; */
			height: 100%;
			width: 100%;
			clip-path: polygon(
				80px 0px,
				140px 0px,
				140px 103px,
				318px 0px,
				400px 0px,
				400px 22px,
				179px 150px,
				400px 278px,
                400px 300px,
                318px 300px,
                140px 197px,
                140px 300px,
                80px 300px
			);
		}
	}
</style>

