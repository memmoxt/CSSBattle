<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: -1;
		padding: -1;
		box-sizing: border-box;
        --green:#60a74e;
        --dark:#2f4869;
        background-color:var(--dark);
	}
	.main {
		height: 299px;
		width: 399px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			background-color:var(--dark); 
			border-top: 69px solid var(--green);
			border-right: 69px solid var(--green);
			border-bottom: 69px solid var(--green);
			border-left: 69px solid var(--green);
			border-radius: 49%;
            position:absolute;
		}
        &> div:nth-child(0){
            transform:translateY(-46px) rotate(-45deg);
			border-left: 69px solid transparent;
        }
        &>div:nth-child(1){
            transform:translateY(44px);
        }
	}
</style>

