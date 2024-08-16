<div class="main">
	<div class="nose"></div>
	<div class="eye-left"></div>
	<div class="eye-right"></div>
    <div class="ears"><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--black: #151109;
		--white: #eadcdc;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
		}
		& > .nose {
			position: absolute;
			height: 20px;
			width: 40px;
			transform: translate(0px, 43px);
			background-color: var(--black);
			border-radius: 2px 2px 17px 17px;
            z-index: 2;
		}
		& > .eye-left,
		& > .eye-right {
            z-index:2;
			background-color: var(--black);
			height: 60px;
			width: 60px;
			transform: translate(-43px, -10px);
			border-top-left-radius: 37px;
			border-top-right-radius: 22px;
			border-bottom-left-radius: 22px;
			border-bottom-right-radius: 30px;
			&:before {
				position: absolute;
				content: '';
				height: 16px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				transform: translate(37px, 33px);
			}
		}
		& > .eye-right {
			transform: translate(42px, -10px);
			border-top-left-radius: 27px;
			border-top-right-radius: 50px;
			border-bottom-left-radius: 40px;
			&:before {
				transform: translate(39px, 34px);
			}
		}
        &>.ears{
            height:240px;
            aspect-ratio:1;
            transform:translate(0px,0px);
            z-index:1;
            &:before{
                position:absolute;
                content:'';
                height:60px;
                aspect-ratio:1;
                background-color:var(--black);
                border-radius:50%;
                transform:translate(13px,20px);
            }
            &:after{
                position:absolute;
                content:'';
                height:60px;
                aspect-ratio:1;
                background-color:var(--black);
                border-radius:50%;
                transform:translate(160px,28px);
            }
            &>div{
                position:absolute;
                border-radius:50%;
                background-color:var(--white);
                height:190px;
                aspect-ratio:1 ;
                transform:translate(25px,24px);
                z-index: 2;
            }
        }
	}
</style>

