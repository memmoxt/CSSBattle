<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #eed9d9;
		--red: #66284a;
        background-color:var(--white);
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
			height: 140px;
			width: 300px;
			position: relative;
			display: flex;
			justify-content: space-between;
			& > div {
				position: relative;
				height: 140px;
				width: 80px;
				background-color: var(--red);
				border-radius: 10px/10px;
				&:before {
					content: '';
					position: absolute;
					height: 50px;
					aspect-ratio: 1;
					background-color: var(--white);
					border-radius: 50%;
                    transform:translate(15px,15px)
				}
                &:after{
                    content:'';
                    position:absolute;
                    height:10px;
                    width:60px;
                    background-color:var(--white);
                    transform:translate(10px,115px);
                    box-shadow:0 -20px var(--white)
                }
			}
		}
	}
</style>
