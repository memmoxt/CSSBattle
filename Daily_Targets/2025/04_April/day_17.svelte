<div class="main">
	<div></div>
    <div></div>
    <div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #d96c7b;
		--white: #ffffff;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--red);
		& > div {
			position: absolute;
			border-top: 20px solid transparent;
			border-right: 20px solid transparent;
			border-bottom: 20px solid transparent;
			border-left: 20px solid var(--white);
			border-radius: 50%;
            transform:rotate(-45deg);
		}
        &>div:nth-child(2){
			border-top: 40px solid transparent;
			border-right: 40px solid transparent;
			border-bottom: 40px solid transparent;
			border-left: 40px solid var(--white);
            transform:rotate(-135deg);
        }
        &>div:nth-child(3){
			border-top: 80px solid transparent;
			border-right: 80px solid transparent;
			border-bottom: 80px solid transparent;
			border-left: 80px solid var(--white);
            transform:rotate(135deg);
        }
        &>div:nth-child(4){
			border-top: 120px solid transparent;
			border-right: 120px solid transparent;
			border-bottom: 120px solid transparent;
			border-left: 120px solid var(--white);
            transform:rotate(45deg);
        }

	}
</style>

