<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --light:#c3d1a5;
        --dark:#374812;
        background-color:var(--light);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div:nth-child(1){
            top:0;
            left:0;
            position:absolute;
            height:210px;
            aspect-ratio:1;
            background-color:var(--dark);
        }
        &>div:nth-child(2){
            position:absolute;
            top:0;
            left:0;
            height:50px;
            aspect-ratio:1;
            background-color:var(--light);
            box-shadow: 105px 55px 0px 25px var(--light),
                55px 105px 0px 25px var(--light),
                160px 160px 0 0 var(--light);
        }

	}
</style>

