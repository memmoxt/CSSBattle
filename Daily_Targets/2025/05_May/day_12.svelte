<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --black:#30383F;
        --pink:#ED6A9D;
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
        &>div{
            position:absolute;
            height:180px;
            aspect-ratio:1;
            background-color:var(--black);
            transform:translate(0px, -50px);
            border-radius:50%;
            &:before{
                content:'';
                position:absolute;
                height:80px;
                width:60px;
                background-color:var(--black);
                transform:translate(60px,90px);
                box-shadow:0 0 0 60px var(--pink), 0 0 0 120px var(--black);
                clip-path:polygon( -120px -0px ,180px -0px, 180px 200px, -120px 200px);
            }
        }

	}
</style>
