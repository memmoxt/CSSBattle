<div class="main">
	<div>
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
		box-sizing: content-box;
		--dark: #2a2753;
		--green: #5a9f48;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--green);
		& > div {
			height: 100px;
			width: 260px;
            clip-path:polygon(0 0 , 100% 0px , 50% 100%);
			display: grid;
			column-gap: 30px;
			grid-template-columns: 45px 40px 40px 45px;
			grid-template-rows: 1fr;
            &>div{
                background-color:var(--dark);
            }
		}
	}
</style>

