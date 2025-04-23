<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #14313e;
		--red: #ba3e46;
		--orange: #f3695a;
		--yellow: #f3ac3c;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--green);
		& > div:nth-child(1) {
			position: absolute;
			background-color: var(--orange);
			height: 30px;
			width: 80px;
			transform: translate(0px, -25px);
			border-radius: 50%;
            z-index:2;
            &:before{
                content:'';
                position:absolute;
                height:30px;
                width:60px;
                background-color:var(--green);
                border-radius:50%;
                transform:translate(10px,-10px);

            }
			&:after {
				content: '';
				height: 50px;
				width: 30px;
				background-color: var(--yellow);
				position: absolute;
				transform: translate(40px, -50px);
				border-top-left-radius: 50px;
				border-bottom-right-radius: 50px;
			}
		}
        &>div:nth-child(2){
            position:absolute;
            height:130px;
            width:80px;
            background-color:var(--red);
            transform:translate(0 , 25px);
            border-radius: 50px/20px;
        }
	}
</style>
