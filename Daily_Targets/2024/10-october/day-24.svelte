<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #434b92;
		--yellow: #f3ac3c;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        overflow: hidden;
		& > div {
			position: absolute;
			height: 100px;
			width: 190px;
			background-color: var(--yellow);
			&:before {
				position: absolute;
				content: '';
				height: 300px;
				width: 50px;
                transform:translate(70px, -100px);
				background-color: var(--yellow);
			}
		}
		& > div:nth-child(2) {
			transform: rotate(90deg);
            &:before{
                height:400px;
                transform:translate(70px, -150px);
            }
		}
	}
</style>

