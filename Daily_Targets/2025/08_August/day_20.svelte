<div class="main">
	<div class="petal"></div>
	<div class="petal"></div>
	<div class="petal"></div>
	<div class="petal"></div>
    <div class="box"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #414b81;

		--yellow: #fade8b;
        background: var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        &>div{
            background-color: var(--yellow);
        }
		& > .petal {
			position: absolute;
			height: 100px;
			aspect-ratio: 1;
			translate: -90px -75px;
			border-radius: 50%;
			border-bottom-right-radius: 0px;
		}
		& > div:nth-child(2) {
			translate: 90px -75px;
			transform: scaleX(-1);
		}
		& > div:nth-child(3) {
			translate: 90px 75px;
			transform: scale(-1);
		}
		& > div:nth-child(4) {
			translate: -90px 75px;
			transform: scaleY(-1);
		}
        &> .box {
            height:50px;
            width:80px;
        }
	}
</style>
