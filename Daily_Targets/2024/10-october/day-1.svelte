<div class="main">
	<div><div></div></div>
	<div><div></div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--grey: #3f4869;
		--yellow: #f4da64;
		--red: #e25c57;
        background-color:var(--grey);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap-reverse;
		flex-direction: column;

		& > div:nth-child(1),
		div:nth-child(2) {
			height: 120px;
			transform: translate(30px, 0px);
			aspect-ratio: 1;
			background-color: var(--grey);
			overflow: hidden;
			& > div {
				height: 120px;
				aspect-ratio: 1;
				background-color: var(--grey);
				transform: translate(-50%, 50%);
				border-radius: 50%;
				box-shadow: 0 0 0 60px var(--red);
			}
		}
		& > div:nth-child(2) {
			transform: translate(-30px) scaleX(-1);
		}
        &> div:nth-child(3){
            position:absolute;
            height:60px;
            aspect-ratio:1;
            background-color:var(--yellow);
            transform:translate(60px,90px);
        }
	}
</style>

