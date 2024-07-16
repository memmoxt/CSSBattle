<div class="main">
    <div></div>
    <div></div>
    <div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
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
		--dark-blue: #243d83;
		--blue: #6592cf;
        background:var(--dark-blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 50px;
			aspect-ratio: 1.2;
			border-radius: 35px/30px;
			background-color: var(--blue);
			transform: translate(0, -60px);
		}
        
        &>div:nth-child(1){
            z-index:2;
        }
        &>div:nth-child(2){
            transform:translate(40px,-40px) rotate(45deg);
            z-index:2;
        }
        &>div:nth-child(3){
            transform:translate(60px,0px) rotate(90deg);
        }
        &>div:nth-child(4){
            transform:translate(40px,40px) rotate(135deg);
        }
        &>div:nth-child(5){
            transform:translate(0px,60px);
        }
        &>div:nth-child(6){
            transform:translate(-40px,40px) rotate(45deg);
        }
        &>div:nth-child(7){
            transform:translate(-60px,0px) rotate(90deg);
        }
        &>div:nth-child(8){
            transform:translate(-40px,-40px) rotate(-45deg);
            z-index:2;
        }
        &>div:nth-child(9){
            height:90px;
            transform:translate(0px,-5px);
        }
        &>div:nth-child(10){
            height:80px;
            width:60px;
            border-radius:0px 0px 60px 60px;
            transform:translate(0px,-15px);
            background-color:var(--dark-blue);
        }
        &>div:nth-child(11),&>div:nth-child(12){
            height:10px;
            aspect-ratio:1;
            border-radius:50%;
            transform:translate(10px,-15px);
            background-color:var(--blue);
        }
        &>div:nth-child(12){
            transform:translate(-10px,-15px);
        }
	}
</style>

