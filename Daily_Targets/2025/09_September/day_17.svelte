<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
        --yellow:#FAE29E;
        --green:#4A9A86;
        background-color:var(--yellow);
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
			height: 420px;
			aspect-ratio: 1;
			background-color: var(--green);
			border-radius: 50%;
            &:before,&:after{
                content:'';
                position:absolute;
                height: 220px;
                border-radius:50%;
                aspect-ratio: 1;
                background-color: transparent;
                translate: 170px 100px;
                box-shadow: 0 0 0 30px var(--yellow);
                clip-path:polygon(-50px -50px, 110px -50px, 110px 250px, -50px 250px);
            }
            &:after{
                transform:scaleX(-1);
                translate:30px 100px;
            }
		}
	}
</style>
