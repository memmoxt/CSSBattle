<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --purple:#62306d;
        --yellow:#f7ec7d;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        overflow: hidden;
        &>div:nth-child(1){
            height:80px;
            width:100px;
            border-radius:50%;
            transform:translate(72px);
            background-color:var(--yellow);
            box-shadow:-72px 0 0 0px var(--purple), -144px 0 0 0 var(--yellow);
        }
	}
</style>

