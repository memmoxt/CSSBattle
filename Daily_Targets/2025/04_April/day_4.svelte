<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--pink: #ffeeee;
		--green: #56ae68;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        margin:0;
        gap:0;
        background-color:var(--pink);
		& > div:nth-child(1) {
			height: 210px;
			width: 174px;
			background-color: var(--pink);
			transform: translate(-33px, 0px);
			/* opacity: 0.5; */
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 250px;
				background-color: var(--green);
				box-shadow: 0 110px 0 var(--green);
			}
			&:after {
				content: '';
				position: absolute;
				height: 210px;
				width: 30px;
				background-color: var(--green);
			}
		}
        &>div:nth-child(2){
            height:210px;
            width:66px;
            right:80px;
            /* background-color:red; */
            /* opacity:0.5; */
            position:absolute;
            overflow: hidden;
            &:before{
                content:'';
                position:absolute;
                border-radius:50%;
                transform:translate(-45px,30px);
                height:80px;
                aspect-ratio:1;
                background-color:var(--pink);
                box-shadow:0 0 0 30px var(--green);
            }
            &:after{
                content:'';
                position:absolute;
                height:120px;
                width:50px;
                transform: translate(-14px, 140px);
                border-top-right-radius:40px;
                box-shadow:0 0 0 30px var(--green);
                background-color:var(--pink);
            }
        }
	}
</style>

