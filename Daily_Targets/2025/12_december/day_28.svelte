<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--darkgreen: #1a552b;
		--green: #74b15c;
        background-color:var(--green);
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
			height: 60px;
			width: 150px;
			background-color: var(--darkgreen);
			translate: -95px -80px;
			box-shadow:
				0px 80px var(--darkgreen),
				0px 160px var(--darkgreen),
				190px 0px var(--darkgreen),
				190px 80px var(--darkgreen),
				190px 160px var(--darkgreen);
            &:before{
                content:'';
                position:absolute;
                height: 300px;
                width: 60px;
                background-color: var(--darkgreen);
                translate: 60px -40px;
                box-shadow:160px 0px var(--darkgreen);
            }
		}
	}
</style>
