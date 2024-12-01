<div class="main">
	<div></div>
    <div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #0b2429;
		--blue: #4a7d7b;
        background-color:var(--green);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			position: absolute;
			top: 110px;
			border-top: 80px solid var(--blue);
			border-right: 50px solid var(--green);
			border-bottom: 0px solid var(--green);
			border-left: 50px solid var(--green);
		}
        &>div:nth-child(2){
            left:50px;
            transform:scaleY(-1);
        }

        &>div:nth-child(3){
            right:50px;
            transform:scaleY(-1);
        }
	}
</style>

