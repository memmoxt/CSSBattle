<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --yellow:#e8ba79;
        --rose:#de817e;
        --purple:#7e6293;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div:nth-child(1){
            position:absolute;
            height:120px;
            aspect-ratio:1;
            border-radius:50%;
            background-color:var(--purple);
            box-shadow:0 0 0px 45px var(--yellow);
            clip-path: polygon( -100px -100px , 200px -100px , 200px 60px, -100px 60px);
        }
        &>div:nth-child(2){
            position:absolute;
            background-color:transparent;
            border-radius:50%;
            border-top: 60px solid var(--rose);
            border-right: 60px solid var(--rose);
            border-bottom: 60px solid transparent;
            border-left: 60px solid transparent;
            transform:rotate(135deg);
        }

	}
</style>

