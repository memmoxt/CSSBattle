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
        --green:#588A95;
        --white:#FFFFFF;
        --black:#222222;
        background-color: var(--green);
        &>div{
            position:absolute;
            height: 140px;
            aspect-ratio:1;
            background-color:var(--black);
            &:before{
                content:'';
                position:absolute;
                height: 140px;
                aspect-ratio: 1;
                background-color: var(--white);
                transform: skewX(45deg);
            }
        }
	}
</style>
