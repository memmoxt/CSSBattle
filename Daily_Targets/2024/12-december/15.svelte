<div class="main">
	<div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f0f0f0;
		--red: #e05947;
        background-color:var(--white);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			height: 200px;
			width: 250px;
			background-color: var(--red);
			overflow: hidden;
			position: absolute;

			& > div:nth-child(1) {
				position: absolute;
				top: 30px;
				left: 30px;
				height: 140px;
				width: 150px;
				background-color: var(--white);
                z-index: 1;
			}
            &>div:nth-child(2){
                position:absolute;
                height:140px;
                top:30px;
                border-radius:50%;
                aspect-ratio:1;
                background-color:var(--white);
                z-index: 2;
                right:-70px;
                box-shadow: 0 0 0 30px var(--red);
            }
		}
	}
</style>

