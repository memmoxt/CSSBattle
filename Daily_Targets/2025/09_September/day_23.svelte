<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f7fcdc;
		--teal: #8ab8b6;
		--magenta: #9f6766;
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
			position: absolute;
			height: 240px;
			aspect-ratio: 1;
			background-color: var(--white);
            translate:0 10px;
            box-shadow: 0 0 0 20px var(--magenta);
            clip-path: polygon(-20px -20px ,260px -20px, 260px 240px, -20px 240px);
            &:before{
                content:'';
                position:absolute;
                height: 50px;
                width:20px;
                background-color: var(--magenta);
                translate: 30px 170px;
                box-shadow: 160px 0 var(--magenta);
            }
            &:after{
                content:'';
                position:absolute;
                height: 150px;
                width: 280px;
                background-color: var(--teal);
                translate: -20px 40px;
            }
		}
	}
</style>
