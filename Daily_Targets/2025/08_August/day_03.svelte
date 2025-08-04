<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
        --white:#FFFFFF;
        --blue:#243D83;
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
			height: 120px;
			aspect-ratio: 1;
			background-color: var(--white);
			translate: -30px -30px;
            box-shadow: 60px 60px var(--white);
            &:before{
                content:'';
                position:absolute;
                height:80px;
                aspect-ratio:1;
                background-color:var(--blue);
                translate:20px 20px;
                box-shadow: 60px 60px var(--blue);  
            }
		}
	}
</style>
