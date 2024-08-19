<div class="main">
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
		--yellow: #eddf5a;
		--blue: #0e127d;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			position: absolute;
			height: 140px;
			width: 50px;
			background-color: var(--blue);
			transform: translate(-25px, 0px);
		}
		& > div:nth-child(2) {
			height: 220px;
			width: 60px;
			background-color: var(--blue);
			transform: translate(20px, 0px);
		}
        &>div:nth-child(3){
            position:absolute;
            height:100px;
            width:20px;
            background-color:var(--yellow);
            transform:translate(-20px,0px);
        }
        &>div:nth-child(4){
            position:absolute;
            height:180px;
            width:20px;
            background-color:var(--yellow);
            transform:translate(20px,0px);
            &:before{
                position:absolute;
                content:'';
                height:20px;
                width:50px;
                background-color:var(--yellow);
                transform:translate(-35px,80px);
            }
        }
	}
</style>

