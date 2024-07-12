<div class="main">
    <div>
    </div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --dark:#243d83;
        --light:#6592cf;
        background-color:var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        
        &>div{
            height:100px;
            width:250px;
            clip-path:path("M 0,0 v100 h100 L60,0 Z M 100,100 200,100 200,0 h-60 Z");
            background-color:var(--light);
        }
        &>div:nth-child(1){
            align-self:start;
            justify-self: start;
        }
        &>div:nth-child(2){
            align-self: end;
            justify-self:end;
            transform:scaleY(-1);
        }
	}
</style>

