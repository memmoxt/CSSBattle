<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--pink: #eed9d9;
		--green: #668884;
        background-color:var(--pink);
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
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--pink);
			/* opacity: 0.5; */
			border-radius: 50%;
			box-shadow: 0 0 0 30px var(--green);
            z-index: 1;
		}
		& > div:nth-child(1) {
			transform: translateX(-40px);
			&:before {
				content: '';
				position: absolute;
				top: -60px;
				border-radius:50%;
				box-shadow: 0 0 0 30px var(--green);
				border-top: 30px solid var(--pink);
				border-right: 30px solid yellow;
				border-bottom: 30px solid yellow;
				border-left: 30px solid yellow;
				transform:rotate(-45deg);
				clip-path: polygon(-60px -60px, 120px -60px, 30px 30px, -0px 0px);
			}
            &:after{
                content:'';
                position:absolute;
                height:60px;
                width:30px;
                left:-30px;
                top:-31px;
                background-color:var(--green);
            }
		}
		& > div:nth-child(2) {
			background-color: var(--green);
            z-index: 2;
			box-shadow: 0 0 0 30px var(--pink);
		}
		& > div:nth-child(3) {
			transform: translateX(40px);
		}
	}
</style>

