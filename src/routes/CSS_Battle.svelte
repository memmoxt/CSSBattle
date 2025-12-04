<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --yellow:#E8AD6D;
        --green:#2F5A76;
        --red:#DE6B67;
        background-color: var(--yellow);
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
            height: 100px;
            width: 280px;
            background-color:var(--red);
            &:before{
                content:'';
                position:absolute;
                height: 160px;
                aspect-ratio:1;
                background-color: var(--green);
                translate: 60px -30px;
            }
            &:after{
                content:'';
                position:absolute;
                height: 100px;
                width: 40px;
                background-color: var(--yellow);
                translate: 120px;

            }
            
        }
	}
</style>
