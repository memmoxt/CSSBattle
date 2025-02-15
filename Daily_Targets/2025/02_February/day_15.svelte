<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fade8b;
		--green: #61a74e;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			transform: translate(0px, -36px);
			height: 200px;
			width: 200px;
			background-color: var(--green);
			&:before {
				content: '';
				position: absolute;
				background-color: var(--yellow);
				top: 155px;
				left: 80px;
				height: 45px;
				width: 40px;
			}
            &:after{
                content:'';
                position:absolute;
                top:200px;
                left:-20px;
                height:90px;
                width:240px;
                background-color:var(--green);
            }
		}
	}
</style>

