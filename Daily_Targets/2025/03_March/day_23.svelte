<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffff;
		--green: #1a353c;
		--yellow: #e0b673;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1) {
			position: absolute;
			top: 39px;
			height: 125px;
			width: 240px;
			/* opacity: 0.5; */
			background-color: var(--green);
            clip-path:polygon(0px 100% , 100px 0px, 140px 0px, 100% 100%);
			&:before {
				content: '';
				position: absolute;
				top: 14px;
				height: 14px;
				width: 40px;
				left: 100px;
				box-shadow:
					0 14px var(--yellow),
					0 28px var(--yellow),
					0 42px var(--yellow),
					0 56px var(--yellow);
				background-color: var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				bottom: -50px;
				left: 70px;
			}
		}
        &>div:nth-child(2){
            position:absolute;
            height:136px;
            width:200px;
            background-color:var(--green);
            /* opacity:0.5; */
            bottom:0px;
        }
	}
</style>

