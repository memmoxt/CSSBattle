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
		box-sizing: border-box;
		--sky: #7dddeb;
		--blue: #4763b1;
        background-color: var(--sky);
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
			position: absolute;
			height: 180px;
			border-radius: 50%;
			aspect-ratio: 1;
			background-color: var(--blue);
			clip-path: polygon(-90px 0px, 90px 0px, 90px 180px, -90px 180px);
		}
        &>div:nth-child(1){
            translate: 90px;
        }
        &>div:nth-child(2){
            translate: 190px;
        }
        &>div:nth-child(3){
            translate: -190px;
            transform: scale(-1);
        }
        &>div:nth-child(4){
            translate:-90px;
            transform:scale(-1);
        }
	}
</style>
