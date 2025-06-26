<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --white:#D9D9D9;
        --blue:#243D83;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        
        &>div{
            height:104px;
            aspect-ratio:1;
            background-color:var(--white);
            border-radius:50%;
            translate:-110px -14px;
            box-shadow: 220px 0 var(--white);
            &::before{
                content:'';
                position:absolute;
                height:110px;
                width:68px;
                translate:36px 22px;
                border-radius:50px/50px;
                background-color:var(--white);
                box-shadow: 184px 0 var(--white);
            }
            &::after{
                content:'';
                position:absolute;
                height:20px;
                aspect-ratio:1;
                background-color:var(--white);
                border-radius:50%;
                translate:124px 42px;
                box-shadow: 56px 0 var(--white);
            }
        }
	}
</style>
