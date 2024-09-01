<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #4a9a86;
		--yellow: #fae29e;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;

		& > div {
			height: 150px;
			width: 250px;
			display: grid;
			grid-template-rows: repeat(3, 50px);
			grid-template-columns: repeat(5, 50px);
            align-content:center;
            &>div{
                height:50px;
                aspect-ratio:1;
                background-color:var(--yellow);
            }
            &>div:nth-child(1){
                grid-column-start:2;
            }
            &>div:nth-child(2){
                grid-column-start:4;
            }
            &>div:nth-child(3){
                grid-column-start:1;
            }
            &>div:nth-child(4){
                grid-column-start:3;
            }
            &>div:nth-child(5){
                grid-column-start:5;
            }
            &>div:nth-child(6){
                grid-column-start:2;
            }
            &>div:nth-child(7){
                grid-column-start:4;
            }
		}
	}
</style>

