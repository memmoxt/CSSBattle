<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --green:#61a74e;
        --dark:#3f4869;
        background-color:var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			background-color:var(--dark); 
			border-top: 70px solid var(--green);
			border-right: 70px solid var(--green);
			border-bottom: 70px solid var(--green);
			border-left: 70px solid var(--green);
			border-radius: 50%;
            position:absolute;
		}
        &> div:nth-child(1){
            transform:translateY(-45px) rotate(-45deg);
			border-left: 70px solid transparent;
        }
        &>div:nth-child(2){
            transform:translateY(45px);
        }
	}
</style>
