<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --green:#5DCBA3;
        --purple:#6255AA;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--purple);
        &>div{
            position:absolute;
            height:50px;
            width:350px;
            background-color:var(--green);
            &:before{
                content:'';
                position:absolute;
                height:50px;
                width:50px;
                background-color:var(--green);
                transform:translate(250px,50px);
                box-shadow: 50px 50px var(--green), 0px -100px var(--green), 50px -150px var(--green);
            }
        }
	}
</style>

