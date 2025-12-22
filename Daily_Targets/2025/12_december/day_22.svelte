<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --red:#ED736E;
        --white:#FEF6E2;
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
        &>div{
            height: 120px;
            aspect-ratio:1;
            background-color: var(--red);
            translate: -140px -65px;
            box-shadow: 280px 130px var(--red);
            &:before{
                content:'';
                height: 200px;
                aspect-ratio:1;
                /* background-color:black; */
                background-color: var(--white);
                border-radius:50%;
                position:absolute;
                translate: 100px 25px;
            }
        }
	}
</style>
