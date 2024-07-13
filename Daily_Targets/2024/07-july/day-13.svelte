<div class="main">
    <div></div>
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
        --orange:#f48b26;
        --yellow:#feff58;
        background:var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: start;
        gap:0 20px;
        &>div{
            height:200px;
            width:30px;
            background-color:var(--yellow);
        }
        &>div:nth-child(2),
        &>div:nth-child(4){
            height:250px;
        }
        &>div:nth-child(3){
            height:300px;
        }
	}
</style>

