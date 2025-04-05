<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #e8ad6d;
		--red: #de6b67;
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
		& > div:nth-child(1){
			height: 200px;
			width: 20px;
			position: absolute;
			background-color: var(--red);
			/* opacity: 0.5; */
			transform: rotate(45deg);
			&:before {
				content: '';
				position: absolute;
				height: 150px;
				aspect-ratio: 1;
				background-color: var(--red);
				/* opacity: 0.5; */
				border-radius: 50%;
				transform: translate(-65px, 25px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 200px;
				width: 20px;
				background-color: var(--red);
                transform: rotate(90deg);
			}
		}
        &>div:nth-child(2){
            height:20px;
            aspect-ratio:1;
            background-color:var(--yellow);
            position:absolute;
            transform:rotate(45deg);
        }
	}
</style>

