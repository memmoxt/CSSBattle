<div class="main">
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
		--black: #000000;
		--white: #ffffff;
        background-color: var(--black);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1) {
			position: absolute;
			top: 110px;
			height: 100px;
			width: 150px;
			background-color: var(--white);
			border-radius: 50px/50px;
			box-shadow: 0 0 0 10px var(--black);
			/* opacity: 0.5; */
            z-index:2;
            &:before,&:after{
                content:'';
                position:absolute;
                transform:translate(20px, 30px) rotate(-30deg);
                border-radius: 50%;
                height:40px;
                width:50px;
                background-color:var(--black);
            }
            &:after{
                transform:translate(80px, 30px) rotate(30deg);
            }
		}
		& > div:nth-child(2),
		& > div:nth-child(3),
		& > div:nth-child(4),
		& > div:nth-child(5) {
			position: absolute;
			height: 40px;
			width: 20px;
			background-color: var(--white);
			/* opacity: 0.5; */
			transform: translate(-80px, -40px) rotate(-45deg);
            z-index:1;
			&:before {
				position: absolute;
				content: '';
				height: 25px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				transform: translate(-10px, -3px);
				box-shadow: 15px 0 var(--white);
			}
		}
        &>div:nth-child(3){
			transform: translate(80px, -40px) rotate(45deg);
        }
        &>div:nth-child(4){
			transform: translate(80px, 60px) rotate(135deg);
        }
        &>div:nth-child(5){
			transform: translate(-80px, 60px) rotate(-135deg);
        }
        &>div:nth-child(6){
            position:absolute;
            height:25px;
            width:15px;
            background-color:var(--white);
            transform:translate(0px ,77px);
            box-shadow:20px 0 var(--white), -20px 0 var(--white);
            /* opacity:0.5; */
        }
	}
</style>

