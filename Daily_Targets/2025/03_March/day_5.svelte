<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #6255aa;
		--red: #d96e9f;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		/* overflow: hidden; */
		& > div {
			position: absolute;
			height: 150px;
			width: 200px;
			background-color: var(--red);
			/* background-color: blue; */
			/* opacity: 0.5; */
			transform: translate(-50%, -50%);
			clip-path: polygon(48px 120px, 142px 0px, 170px 37px, 170px 120px);
		}
        &>div:nth-child(2){
            transform:translate(50%,-50%) scaleX(-1);
        }
        &>div:nth-child(3){
            transform:translate(-50%,50%) scaleY(-1);

        }
        &>div:nth-child(4){
            transform:translate(50%,50%) scale(-1);

        }
	}
</style>

