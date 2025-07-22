<div class="main">
	<div class="eye"></div>
	<div class="eye"></div>
    <div class="body"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #439e6b;
		--dark: #246541;
		--white: #eeeeee;
		--black: #000000;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > .eye {
			position: absolute;
			height: 50px;
			aspect-ratio: 1;
			background-color: var(--white);
			border-radius: 50%;
			translate: -25px -80px;
            overflow:hidden;
            z-index:1;
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				aspect-ratio: 1;
				background-color: var(--black);
				border-radius: 50%;
				translate: 15px 7px;
			}
            &:after{
                content:'';
                position:absolute;
                height:17px;
                width:100px;
                background-color: var(--green);
                box-shadow: 0 33px var(--green);
            }
            
		}


        &> .eye:nth-child(2){
            transform:translate(50px);

        }
        &>.body{
            position:absolute;
            height:160px;
            width:100px;
            background-color: var(--dark);
            &:before{
                content:'';
                position:absolute;
                height: 14px;
                width:30px;
                background-color:var(--green);
                translate:-30px 130px;
                box-shadow: 130px 0 var(--green);
            }
            &:after{
                content:'';
                position:absolute;
                height: 40px;
                width: 14px;
                background-color:var(--green);
                translate: -30px 130px;
                box-shadow: 146px 0 var(--green);
            }
        }
	}
</style>
