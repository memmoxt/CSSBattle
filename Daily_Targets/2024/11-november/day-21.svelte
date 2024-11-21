<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #63a3a0;
		--white: #f3ead2;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--green);
        &>div{
            position:absolute;
            height:100px;
            width:120px;
            background-color:var(--white);
            border-radius:50%;
            top:45px;
            &:before{
                position:absolute;
                content:'';
                left:10px;
                top:90px;
                height:120px;
                width:100px;
                background-color:var(--white);
            }
            &:after{
                position:absolute;
                content:'';
                bottom:-110px;
                height:20px;
                width:120px;
                background-color:var(--white);
            }

        }

	}
</style>

