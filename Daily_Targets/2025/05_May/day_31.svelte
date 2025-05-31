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
		--orange: #f3ac3c;
		--black: #282828;
        background-color:var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1),div:nth-child(2) {
			position: absolute;
			background-color: var(--black);
			height: 40px;
			width: 20px;
			transform: translate(0px, 60px);
			transform-origin: -20px -10px;
			box-shadow: 0 -120px var(--black);
		}
		& > div:nth-child(2) {
			transform: rotate(90deg);
		}
		& > div:nth-child(3),div:nth-child(4) {
            background-color:var(--black);
            height:40px;
            width:20px;
            transform:translate(80px,70px) rotate(-45deg);
            box-shadow:0px -200px var(--black);
		}
        &> div:nth-child(4){
            transform:translate(-80px,70px) rotate(45deg);
        }
	}
</style>
