<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #51a499;
		--yellow: #eac049;
        --black:#282828;
        background-color:var(--green);
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
			position: absolute;
			height: 120px;
			aspect-ratio: 1;
			background-color: var(--yellow);
			box-shadow:
				-40px 0px var(--yellow),
				40px 0px var(--yellow),
				0px -40px var(--yellow),
                0px 40px var(--yellow);
            &:before,&:after{
                content:'';
                position:absolute;
                height:200px;
                width:40px;
                transform:translate(40px, -40px);
                background-color:var(--black);
            }
            &:after{
                transform:translate(40px, -40px) rotate(90deg);
            }
		}
	}
</style>
