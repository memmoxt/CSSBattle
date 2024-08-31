<div class="main">
	<div></div>
    <div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fae29e;
		--orange: #ea9a52;
        background-color:var(--yellow);

	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
            position:absolute;
			height: 120px;
			width: 60px;
			border-radius: 50px/50px;
			background-color: var(--orange);
			transform: translate(-95px) rotate(0deg);
		}
        &>div:nth-child(2){
            transform-origin: bottom;
			transform: translate(-4px, 53px) rotate(60deg);
        }
        &>div:nth-child(3){
            transform-origin: bottom;
			transform: translate(100px, -113px) rotate(-60deg);
        }
        
	}
</style>

