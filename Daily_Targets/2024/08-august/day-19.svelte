<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #f2eaa8;
		--green: #98cea1;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div{
            height:200px;
            width:40px;
            background-color:var(--green);
            &:before{
                position:absolute;
                content:'';
                height:200px;
                width:40px;
                background-color:var(--green);
                transform:rotate(90deg);
            }
        }
        &>div:nth-child(2){
            position:absolute;
            transform:rotate(45deg);
        }

	}
</style>

