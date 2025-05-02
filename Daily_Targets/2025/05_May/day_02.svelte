<div class="main">
	<div class="box">
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --white:#FEFAED;
        --purple:#9A5DCB;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color: var(--white);
		& > .box {
            position:absolute;
            height:160px;
            width:240px;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-template-rows: repeat(2, 1fr);
            &>div{
                position:relative;
                height:100%;
                width:100%;
                background-color: var(--purple);
            }
            &>div:nth-child(1){
                grid-column: 1/2;
                grid-row: 2/3;
                border-bottom-right-radius:20px;
                border-top-left-radius:20px;
            }
            &>div:nth-child(2){
                grid-column:2/3;
                grid-row: 1/2;
                border-top-right-radius: 20px;
                border-top-left-radius: 20px;
            }
            &>div:nth-child(3){
                grid-column: 3/4;
                grid-row:-2;
                border-top-right-radius: 20px;
                border-bottom-left-radius: 20px;
            }
		}
	}
</style>
