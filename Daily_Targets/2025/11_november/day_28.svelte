<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --orange:#D86F45;
        --white:#F5D6B4;
        --brown:#734939;
        background-color: var(--orange);

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
            height: 160px;
            width:200px;
            background-color: var(--brown);
            translate: -20px -20px;
            &:before{
                content:'';
                position:absolute;
                height: 160px;
                width: 200px;
                background-color:var(--white);
                border-radius: 20px / 20px;
                translate: 20px 20px;
            }
            &:after{
                content:'';
                position:absolute;
                height: 40px;
                width:100px;
                background-color:var(--orange);
                translate: 140px 60px;
            }
        }
	}
</style>
