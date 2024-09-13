<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --blue:#328FC1;
        --lightblue:#8cd5f5;
        background-color:var(--lightblue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div{
            height:80px;
            width:250px;
            background-color:var(--blue);
            border-radius:50px/50px;
            &:before{
                content:'';
                position:absolute;
                height:60px;
                aspect-ratio:1;
                border-radius:50%;
                background-color:var(--lightblue);
                transform:translate(10px,10px);
                box-shadow: 170px 0 0 var(--lightblue);
            }
        }
	}
</style>

