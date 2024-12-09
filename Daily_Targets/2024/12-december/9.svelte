<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f0dac1;
		--red: #c3463d;
		--dark: #a52f28;
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
            position:absolute;
            left:0;
            top:90px;
            border-top: 90px solid var(--dark);
            border-right: 80px solid var(--white);
            border-bottom: 90px solid var(--dark);
            border-left: 220px solid var(--dark);
            &:before{
                content:'';
                position:absolute;
                height:180px;
                width:140px;
                background-color:var(--red);
                top:-150px;
                left:-220px;
            }
        }
	}
</style>

