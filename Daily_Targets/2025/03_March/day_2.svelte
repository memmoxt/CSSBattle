<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #84b9c7;
		--green: #1a353c;
        background-color:var(--blue);
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

        &:before{
            content:'';
            position:absolute;
            height:29.5px;
            width:320px;
            background-color:var(--green);
            transform:translateY(-35px);
        }
		& > div {
			height: 104px;
			width: 120px;
			background-color: var(--blue);
			/* opacity: 0; */
			position: absolute;
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--blue);
				transform: translate(30px, -30px);
                box-shadow:0 0 0 29.5px var(--green);
			}
            &:after{
                content:'';
                position:absolute;
                height:120px;
                width:30px;
                background-color:var(--green);
                transform:translate(90px,0px);
            }
		}
		& > div:nth-child(1) {
			transform: translate(-100px, 51px);
		}
		& > div:nth-child(2) {
			transform: translate(100px, 51px) scaleX(-1);
		}
	}
</style>


