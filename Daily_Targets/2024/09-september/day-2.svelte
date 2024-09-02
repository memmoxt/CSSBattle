<div class="main">
	<div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing:border-box;
		--blue: #b6ebe7;
		--purple: #9382e4;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        
		& > div {
			background-color: var(--purple);
			height: 200px;
			aspect-ratio: 1;
		}
        &>div:nth-child(2){
            position:absolute;
            height:200px;
            transform:rotate(45deg);
        }
        &>div:nth-child(1){
            display:flex;
            justify-content:center;
            align-items:center;
            &:before{
                content:'';
                position:absolute;
                background-color:var(--blue);
                height:100px;
                aspect-ratio:1;
                z-index: 2;
            
            }
        }
	}
</style>

