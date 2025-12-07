<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #e3516e;
		--brown: #511818;
        background-color: var(--red);
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
			height: 100px;
			width: 220px;
			background-color: var(--brown);
            &:before{
                content:'';
                position:absolute;
                height:80px;
                aspect-ratio:1;
                background-color: var(--red);
                translate: 70px -40px;
            }
            &:after{
                content:'';
                position:absolute;
                height: 40px;
                aspect-ratio:1;
                background-color: var(--brown);
                border-radius:50px;
                translate: 90px -20px;
                box-shadow: 0 140px var(--brown);
            }
		}
	}
</style>
