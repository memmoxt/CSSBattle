<div class="main">
	<div class="center">
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
		box-sizing: content-box;
		--sky: #6592cf;
		--blue: #243d83;
        background:var(--sky);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
		& > .center {
			display: grid;
			grid-template-columns: repeat(4, 60px);
            grid-template-rows: 20px 120px 20px;
            gap:20px;
			height: 200px;
			width: 300px;
            &>div{
                height:20px;
                width:60px;
                background-color:var(--blue);
            }
            &>div:nth-child(3){
                width:140px;
            }
            &>div:nth-child(4){
                height:120px;
                width:300px;
                grid-column: 1/-1;
            }
            &>div:nth-child(5){
                width:140px;
                grid-column:1/3;
            }
		}
	}
</style>

