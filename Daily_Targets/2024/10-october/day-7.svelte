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
		box-sizing: border-box;
        --blue:#6592cf;
        --darkblue:#243d83;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
        grid-template-columns: 1fr 150px 1fr;
        grid-template-rows: 1fr 150px 1fr;
        &>div{
            background-color:var(--darkblue);
            height:100%;
            width:100%;
        }
        &>div:nth-child(1){
            grid-column:2/3;
        }
        &>div:nth-child(2)
        {
            grid-column:2;
            grid-row:3;
        }
        &>div:nth-child(3){
            grid-column:3;
            grid-row:2;
        }
        &>div:nth-child(4){
            grid-column:1;
            grid-row:2;
        }
        &>div:nth-child(5){
            grid-column:2;
            grid-row:2;
            border-radius:50%;
            background-color:var(--darkblue);
            box-shadow: 0 0 0 50px var(--blue);
            z-index: 1;
        }
    
	}
</style>

