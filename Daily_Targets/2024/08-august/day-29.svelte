<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f9ddc6;
		--purple: #594c94;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1) {
			height: 200px;
			width: 250px;
			background-color: var(--purple);
			display: flex;
			justify-content: center;
			align-items: center;
			& > div {
                
				background-color: var(--white);
				height: 100px;
				width: 150px;
                &:before,&:after{
                    position: absolute;
                    content:'';
                    height:20px;
                    width:50px;
                    background-color:var(--white);
                    transform:translate(150px);
                }
                &:after{
                    transform:translate(-15px, 115px) rotate(90deg);
                }
			}
		}
	}
</style>

