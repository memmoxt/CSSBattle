<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #555fd9;
		--orange: #f2a842;
        background-color:var(--blue);
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
			height: 160px;
			width: 100px;
			background-color: var(--blue);
			box-shadow:
				40px 20px var(--orange),
				40px -20px var(--orange),
				-40px 20px var(--orange),
				-40px -20px var(--orange);
            &:before{
                content:'';
                position:absolute;
                height:20px;
                width:90px;
                background-color:var(--orange);
                translate: -150px -20px;
                box-shadow: 310px 0px var(--orange), 0 180px var(--orange), 310px 180px var(--orange);

            }
		}
	}
</style>
