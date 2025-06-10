<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #eeb850;
		--blue: #243d83;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--yellow);
		& > div:nth-child(1) {
			position: absolute;
			height: 200px;
			width: 300px;
			background-color: var(--blue);
			clip-path: polygon(
				0 60px,
				60px 60px,
				60px 0,
				240px 0,
				240px 60px,
				300px 60px,
				300px 200px,
				240px 200px,
				240px 140px,
				60px 140px,
				60px 200px,
				0px 200px
			);
		}
		& > div:nth-child(2) {
			position: absolute;
			transform: translate(0px, -30px);
			height: 100px;
			width: 140px;
			background-color: var(--yellow);
            &:before{
                content:'';
                position:absolute;
                background-color:var(--yellow);
                height:40px;
                width:60px;
                transform:translate(-60px,60px);
                box-shadow:200px 0 var(--yellow);
            }
            &:after{
                content:'';
                position:absolute;
                background-color:var(--yellow);
                height:120px;
                width:20px;
                box-shadow:240px 0 var(--yellow);
                transform:translate(-60px, 60px);
            }
		}
	}
</style>
