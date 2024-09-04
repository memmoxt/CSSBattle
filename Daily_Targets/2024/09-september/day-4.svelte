<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--light: #f3ac3c;
		--dark: #998235;
        background-color:var(--light);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		flex-direction: column;
		align-items: center;
		& > div:nth-child(1) {
			transform: translateY(3px);
			height: 18px;
			width: 80px;
			background-color: var(--dark);
		}
		& > div:nth-child(2) {
			height: 86px;
			width: 105px;
			background-color: var(--dark);
			transform: translate(-27px, 3px);
			border-bottom-left-radius: 30px;
			border-bottom-right-radius: 30px;
			&:before {
				position: absolute;
				content: '';
				height: 79px;
				width: 49px;
				background-color: var(--light);
				transform: translate(6px, 0px);
                border-radius: 0px 0px 50px 50px;
			}
            &:after{
                position:absolute;
                content:'';
                height:55px;
                width:20px;
                background-color:var(--light);
            }
		}
	}
</style>

